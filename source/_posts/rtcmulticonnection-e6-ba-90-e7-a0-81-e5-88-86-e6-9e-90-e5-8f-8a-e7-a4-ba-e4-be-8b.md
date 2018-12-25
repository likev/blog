---
title: RTCMultiConnection源码分析及示例
id: 1386
categories:
  - javascript
date: 2015-02-07 21:58:07
tags:
---

RTCMultiConnection是运行在RTCPeerConnection API之上的WebRTC JavaScript包装库，可以实现基于WebRTC的点对点多人会话，点对点文件分享，以及视频聊天等功能。
下面对RTCMultiConnection的部分源代码(基于 [v2.2.5](https://github.com/muaz-khan/RTCMultiConnection/blob/df1d23d155dfb0e9f4983581043d22d4794c45ae/RTCMultiConnection.js "v2.2.5源码查看"))进行简单分析。

<pre lang='javascript' line="1679">
 var iceServers = [];
iceServers.push({
url: 'stun:stun.l.google.com:19302'
});
iceServers.push({
url: 'stun:stun.anyfirewall.com:3478'
});
iceServers.push({
url: 'turn:turn.bistri.com:80',
credential: 'homeo',
username: 'homeo'
});
iceServers.push({
url: 'turn:turn.anyfirewall.com:443?transport=tcp',
credential: 'webrtc',
username: 'webrtc'
});
connection.iceServers = iceServers;
</pre>
上述源代码配置了STUN和TURN服务器，使用时可以用新的配置覆盖。这个地址列出了可用的 [STUN server list](https://gist.github.com/zziuni/3741933 "STUN server list")

<pre lang='javascript' line="1278">
 // resources used in RTCMultiConnection
connection.resources = {
RecordRTC: 'https://cdn.webrtc-experiment.com/RecordRTC.js',
PreRecordedMediaStreamer: 'https://cdn.webrtc-experiment.com/PreRecordedMediaStreamer.js',
customGetUserMediaBar: 'https://cdn.webrtc-experiment.com/navigator.customGetUserMediaBar.js',
html2canvas: 'https://cdn.webrtc-experiment.com/screenshot.js',
hark: 'https://cdn.webrtc-experiment.com/hark.js',
firebase: 'https://cdn.webrtc-experiment.com/firebase.js',
firebaseio: 'https://chat.firebaseIO.com/',
muted: 'https://cdn.webrtc-experiment.com/images/muted.png',
getConnectionStats: 'https://cdn.webrtc-experiment.com/getConnectionStats.js',
FileBufferReader: 'https://cdn.webrtc-experiment.com/FileBufferReader.js'
};
// www.RTCMultiConnection.org/docs/body/
connection.body = document.body || document.documentElement;
// www.RTCMultiConnection.org/docs/peers/
connection.peers = {};
// www.RTCMultiConnection.org/docs/firebase/
connection.firebase = 'chat';
</pre>

<pre lang='javascript' line="2451">
 // www.RTCMultiConnection.org/docs/openSignalingChannel/
// http://goo.gl/uvoIcZ
connection.openSignalingChannel = function(config) {
// make sure firebase.js is loaded
if (!window.Firebase) {
return loadScript(connection.resources.firebase, function() {
connection.openSignalingChannel(config);
});
}
var channel = config.channel || connection.channel;
if (connection.firebase) {
// for custom firebase instances
connection.resources.firebaseio = connection.resources.firebaseio.replace('//chat.', '//' + connection.firebase + '.');
}
var firebase = new window.Firebase(connection.resources.firebaseio + channel);
firebase.channel = channel;
firebase.on('child_added', function(data) {
config.onmessage(data.val());
});
firebase.send = function(data) {
// a quick dirty workaround to make sure firebase
// shouldn't fail for NULL values.
for (var prop in data) {
if (isNull(data[prop]) || typeof data[prop] === 'function') {
data[prop] = false;
}
}
this.push(data);
};
if (!connection.socket) {
connection.socket = firebase;
}
firebase.onDisconnect().remove();
setTimeout(function() {
config.callback(firebase);
}, 1);
};
connection.Plugin = Plugin;
};
</pre>

RTCMultiConnection默认使用了 https://chat.firebaseIO.com/ 信号服务，使用时可修改为自己的firebase地址 `connection.firebase = 'yourname';`
也可使用其他服务端信号实现，在客户端重载openSignalingChannel函数，详见 [https://github.com/muaz-khan/WebRTC-Experiment/blob/master/Signaling.md](https://github.com/muaz-khan/WebRTC-Experiment/blob/master/Signaling.md "信号实现方式")的介绍。

完整示例：
<pre lang='javascript'>
<!DOCTYPE html>
<!--

-->

<html>

<head>
  <meta charset="utf-8">
  <title>利用RTCMultiConnection进行基于WebRTC的实时多人点对点文字聊天和文件分享</title>
  <script src="http://www.webrtc-experiment.com/firebase.js"></script>
  <script src="http://www.webrtc-experiment.com/RTCMultiConnection.js"></script>
  <script src="http://www.webrtc-experiment.com/FileBufferReader.js"></script>
</head>

<body>
  <section>

## Open Data Channel

    <input type="text" id="channel" value="channel" style="font-size: 1.1em; text-align: right; width: 4em;" title="channel name - use your own channel name">
    <button id="init-RTCMultiConnection">Open</button>
    <span>or join:</span>
    <button id="join-RTCMultiConnection">Join</button>
  </section>

  <div id="chat-output"></div>
  <input type="text" id="chat-input" style="font-size: 1.2em;" placeholder="chat message" disabled>

## Share Files

  <input type="file" id="file" disabled>

  <div id="file-progress"></div>

  <script>
        var d = document;
        d.$ = document.getElementById;
        d.$('channel').value = Math.round(Math.random() * 60535) + 500000;
        var connection = new RTCMultiConnection();

        connection.session = {
            data: true
        };

        var iceServers = [];
		iceServers.push({
            url: 'stun:stun.services.mozilla.com'
        });

		/* Google服务不通
        iceServers.push({
            url: 'stun:stun.l.google.com:19302'
        });

        iceServers.push({
            url: 'stun:stun.anyfirewall.com:3478'
        });
*/
        iceServers.push({
            url: 'turn:turn.bistri.com:80',
            credential: 'homeo',
            username: 'homeo'
        });

        iceServers.push({
            url: 'turn:turn.anyfirewall.com:443?transport=tcp',
            credential: 'webrtc',
            username: 'webrtc'
        });

        connection.iceServers = iceServers;

        // [optional] onmessage/onopen is for sending/receiving data/text
        connection.onmessage = function(e) {
            appendDIV(e.data);
        };

        connection.onopen = function() {
            if (d.$('chat-input')) d.$('chat-input').disabled = false;
            if (d.$('file')) d.$('file').disabled = false;

            if (d.$('init-RTCMultiConnection')) d.$('init-RTCMultiConnection').disabled = true;
        };

		connection.onerror = function (e) {
			// e.userid
			// e.extra
			 console.log(e);
		}

        d.$('init-RTCMultiConnection').onclick = function() {
            connection.open(d.$('channel').value || 'channel');
            d.$('join-RTCMultiConnection').disabled = true;
            d.$('init-RTCMultiConnection').disabled = true;
        };

        d.$('join-RTCMultiConnection').onclick = function() {
            connection.connect(d.$('channel').value || 'channel');
            d.$('join-RTCMultiConnection').disabled = true;
            d.$('init-RTCMultiConnection').disabled = true;
        };

        d.$('file').onchange = function() {
            var file = this.files[0];
            connection.send(file);
        };

        var chatOutput = d.$('chat-output');

        connection.body = d.$('file-progress');

        function appendDIV(data) {
            var div = document.createElement('div');
            div.innerHTML = data;

            chatOutput.insertBefore(div, chatOutput.firstChild);

            div.tabIndex = 0;
            div.focus();
        }

        d.$('chat-input').onkeypress = function(e) {
            if (e.keyCode !== 13 || !this.value) return;
            appendDIV(this.value);
            connection.send(this.value);
            this.value = '';
            this.focus();
        };
  </script>
</body>

</html>
</pre>

[new RTCMultiConnection](http://www.rtcmulticonnection.org/docs/constructor/ "构造函数")('channel-id');创建一个信道，参数为空时默认信道名为完整URL。
[connection.open](http://www.rtcmulticonnection.org/docs/open/ "创建会话")('session-id'); 在当前信道创建一个会话，可理解为一个房间。一个信道可以有多个房间。
[connection.connect](http://www.rtcmulticonnection.org/docs/connect/ "连接会话")('session-id');连接新的socket或使用已有socket，等待onNewSession事件，然后默认connection.join(session);

RTCMultiConnection官方网站及文档和示例：[http://www.rtcmulticonnection.org/](http://www.rtcmulticonnection.org/ "打开网址")
firebaseAPI：[https://www.firebase.com/docs/web/api/](https://www.firebase.com/docs/web/api/ "打开网址")

* * *

其他基于WebRTC的JavaScript类库

1.  [PeerJS](http://peerjs.com/ "打开官网")简化WebRTC点对点数据、音视频通话。同样需要PeerServer来协商会话双方，可使用官网提供的免费服务。
2.  [rtc.io](https://rtc.io/ "打开官网")是一个node.js的模块集合，可用来简化WebRTC开发
3.  [https://simplewebrtc.com/](https://simplewebrtc.com/ "打开官网")由一些独立的模块构成
4.  [http://sipjs.com/](http://sipjs.com/ "打开官网")和peerjs类似，同样需要SIP服务，可使用他们的付费[OnSIP服务](https://signup.onsip.com/sipjs "注册OnSIP服务")