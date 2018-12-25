---
title: Javascript 中的编码与解码
tags:
  - javascript
  - 参数
  - 字符
  - 文档
  - 编码
  - 解码
id: 720
categories:
  - javascript
date: 2011-08-17 20:54:54
---

1.encodeURI/decodeURI 用于编码/解码整个带参数的URI，比如用函数新打开一个网址  注意参数为整个(或编码后的)url字符串
<pre lang='javascript'>
var url="http://grow.sinaapp.com/?test=a&str='a b+c 编码'";
var out= encodeURI(url);
alert(out);
</pre>
[运行以上代码](#)

2.encodeURIComponent/decodeURIComponent 用于编码解码一个URI组件(url请求参数)，比如ajax请求时的参数  注意参数为URL请求参数的一部分
 <pre lang='javascript'>
var arg="http://grow.sinaapp.com/?test=a&str='a b+c 编码'";
var out= encodeURIComponent(arg);
alert(out);
</pre>
[运行以上代码](#)

3.escape/unescape 对字符串进行编码/解码，用于html文档内部，比如对于文档dom的操作
<pre lang='javascript'>
var str="http://grow.sinaapp.com/?test=a&str='a b+c 编码'";
var out= escape(str);
alert(out);
</pre>
[运行以上代码](#)