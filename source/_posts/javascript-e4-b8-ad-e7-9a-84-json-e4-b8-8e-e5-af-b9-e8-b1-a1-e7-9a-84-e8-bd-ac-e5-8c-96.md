---
title: Javascript 中的 json与对象的转化
tags:
  - javascript
  - json
  - json2.js
  - stringify
  - 字符串
  - 对象
  - 格式
  - 转化
id: 736
categories:
  - html
  - javascript
date: 2011-08-17 22:56:13
---

简单的说json是一种数据交换格式。具体说明请见官方网站[中文站](http://www.json.org/json-zh.html)

将后台程序(如php)发送过来的json数据转化为javascript的数组或者对象的方法十分简单，代码如下
<pre lang='javascript'>
//假设后台发送的json数据为 '{a:2,b:1}' 存储于str中
var data = eval( '(' + str + ')' );
</pre>

然而想**将一个javascript对象转化为json格式的字符串**却并不那么简单，特别是对象的属性值递归包含一个对象时(如 var obj={a:[2,3],b:{m:[3,4],n:2} } ),那么有没有什么方法将obj转化为json格式的字符串呢？

当然你可以自己写一个函数，递归遍历一个对象并将其转化为json格式的字符串，对于大部分人来说这有些困难并容易出错。
幸好已经有人做好了这件事情，你只用包含一段javascript代码即可。
打开官方网站http://www.json.org/json-zh.html ,找到Javascript分类下的 [json2.js](https://github.com/douglascrockford/JSON-js)链接并打开，然后下载文件并解压，在你的网页中包含json2.js文件即可。

使用方法：
<pre lang='html4strict'>
<!doctype html>
<html>
<body>
<script src="json2.js"></script>
<script>
var obj={a:[2,3],b:{m:[3,4],n:2} };
var jsonStr = JSON.stringify( obj );
alert(jsonStr);
//将显示 {"a":[2,3],"b":{"m":[3,4],"n":2}}
</script>
</body>
</html>
</pre>

------------------------------------------------------------
补充：貌似现在新版的浏览器都原生支持JSON.stringify函数了。请见此文介绍：[JSON对象和字符串之间的相互转换](http://www.css88.com/archives/3919)