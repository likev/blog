---
title: Javascript 中 setInterval 和 setTimeout函数的使用感受
tags:
  - javascript
  - 函数
  - 方式
  - 递归
id: 578
categories:
  - javascript
date: 2011-03-09 14:35:30
---

当需要现在执行一个函数并且每10秒钟执行一次这个函数你会怎么做呢，是不是像下面这样

<pre lang='javascript'>
var func = function(){
	//some code
}
func();
window.inter = setInterval(func, 10*1000);
</pre>

有没有其它的方式呢，下面是我最近的写法

<pre lang='javascript'>
var func = function(){
	//some code
	window.out = setTimeout(func, 10*1000);
}
func();
</pre>

本以为code2的方式会更简洁点，但是随后使用的时候就发现问题了，比如如果你想再执行一次这个函数怎么办呢。由于code2的书写方式导致每调用一次func后会造成递归调用，无法停止了。即使clearTimeout(out)也显得有些混乱，因为如果之前连续两次调用func时就会出问题。

以自己的经历给大家一个忠告吧，一个函数尽可能只完成一项功能，像code1那样的方式书写会更好。