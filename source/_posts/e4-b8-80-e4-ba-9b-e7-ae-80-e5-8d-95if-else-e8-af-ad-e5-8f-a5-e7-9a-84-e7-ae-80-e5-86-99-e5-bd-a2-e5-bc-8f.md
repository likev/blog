---
title: 一些简单分支判断语句的简写形式
tags:
  - if else
  - 分支
  - 判断
  - 实现
  - 简写
  - 语句
id: 818
categories:
  - javascript
  - 编程
date: 2011-08-27 01:08:44
---

有一些分支判断语句比较简单，可以不用if else语句来实现。
下面以Javascript语言为例来演示：

<pre lang='javascript'>
var a;
var f = function(m){
	alert(m);
}

//示例一
if(a){
	f();
}
//简写形式
a && f();

//示例二
if(!a){
	f();
}
//简写形式
a || f();

//示例三
if(a>3){
	f(1);
}else{
	f(2);
}
//简写形式
a>3 ? f(1) : f(2);

</pre>