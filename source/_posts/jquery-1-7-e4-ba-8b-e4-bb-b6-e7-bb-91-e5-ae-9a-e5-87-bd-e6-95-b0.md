---
title: jQuery 1.7 事件绑定函数
tags:
  - drop
  - event
  - html5
  - jquery
  - 事件
id: 967
categories:
  - html
  - javascript
date: 2011-11-08 00:32:45
---

jQuery 1.7 前几天发布了，新增了两个事件处理函数 `.on()` 和 `.off()` 分别用来绑定和解除事件。这两个函数可以**取代**之前版本中所有的事件处理函数。
现在事件绑定和解除更简单了，下面是新旧版本事件处理代码的对比：
<pre lang='javascript'>
$('a').bind('click', myHandler);
$('a').on('click', myHandler);

$('form').bind('submit', { val: 42 }, fn);
$('form').on('submit', { val: 42 }, fn);

$(window).unbind('scroll.myPlugin');
$(window).off('scroll.myPlugin');

$('.comment').delegate('a.add', 'click', addNew);
$('.comment').on('click', 'a.add', addNew);

$('.dialog').undelegate('a', 'click.myDlg');
$('.dialog').off('click.myDlg', 'a');

$('a').live('click', fn);
$(document).on('click', 'a', fn);

$('a').die('click');
$(document).off('click', 'a');
</pre>

另外想说一下jQuery中的**事件对象([Event Object](http://api.jquery.com/category/events/event-object/))**：

jQuery的事件系统规范化了事件对象(根据W3C标准)。jQuery保证事件对象被传递给事件处理程序。大部分的属性从原来的事件中复制和规范化给新的事件对象。

jQuery保证下列属性是事件对象的成员，尽管它们中的一些值可能是undefined(依赖于具体的事件):
<pre lang='javascript'>
altKey, attrChange, attrName, bubbles, button, cancelable, 
charCode, clientX, clientY, ctrlKey, currentTarget, data, detail, 
eventPhase, fromElement, handler, keyCode, layerX, layerY,
 metaKey, newValue, offsetX, offsetY, originalTarget,
 pageX, pageY, prevValue, relatedNode, relatedTarget, 
screenX, screenY, shiftKey, srcElement, target, 
toElement, view, wheelDelta, which
</pre>

为了跨浏览器兼容，jQuery 对下列属性进行了规范化:
<pre lang='javascript'>
    target
    relatedTarget
    pageX
    pageY
    which
    metaKey
</pre>

**特别注意**，并不是所有原始事件的属性都被复制给jQuery的事件对象。这时可以用 event.originalEvent 来获取原始事件对象。比如在HTML5文件拖放操作时需要用到drop事件的dataTransfer属性，可以像下面这样做：
<pre lang='javascript'>
$('body').on('drop',function(e){
	var file = e.originalEvent.dataTransfer.files[0];//获取一组拖放文件中的第一个文件

	reader = new FileReader();//创建FileReader对象来读取文件内容
	reader.onload = function(e){//读取完成时将内容显示于body中
		$('body').text(e.target.result);
	};
	reader.readAsText(file,'utf-8');//开始读取文件

	//相当于同时调用e.stopPropagation() 和 e.preventDefault()
	return false;//阻止事件冒泡和浏览器的默认行为
});
</pre>