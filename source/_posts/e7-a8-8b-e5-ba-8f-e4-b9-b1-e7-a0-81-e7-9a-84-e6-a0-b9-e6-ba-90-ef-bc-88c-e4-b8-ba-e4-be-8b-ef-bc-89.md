---
title: 程序乱码的根源（C++为例）
tags:
  - C++
  - 编码
id: 251
categories:
  - C++
date: 2010-09-17 05:24:15
---

当字符以某种编码（例如gbk）存储，但是以另一种编码（例如utf-8）显示时，乱码就产生了。

例如以下的C++源代码
//file1.cpp
<pre lang='cpp'>
#include <iostream>
int main()
{
char str[100]=&quot;abc完美&quot;;
std::cout&lt;&lt;str;
}
</pre>

当编译链接后，程序在控制台（终端）一定会显示 abc完美 这几个字符么，不一定。

首先要看源代码file1.cpp是采用什么编码方式存储的，假如是GBK编码方式，则编译后生成的可执行文件中存储的是"abc完美"的GBK码。

其次要看系统的默认编码是什么，简体中文Windows的系统默认编码是GBK，Ubuntu 10的系统默认编码是UTF-8。当执行程序时，系统会用默认的编码显示字体。

具体来说，如果file1.cpp是用GBK编码方式，则字符串"abc完美"也将以GBK编码存储在可执行程序中，在简体中文Windows中运行程序时，系统将以默认的GBK编码解读字符串，于是正确显示字符串"abc完美"；但是当在Ubuntu 10中运行程序时，系统也将以默认的UTF-8编码解读字符串，由于用以存储和显示字符串的编码方式不一致，于是乱码产生了。

所以如果不考虑跨平带和国际化的话，源代码要以系统默认的编码方式存储，这样可以避免乱码的产生。对于初学者，这应该是比较简单实用的方式。

相关讨论

1.  [所见非所得-C++的代码编码(Encoding)](http://zadecn.spaces.live.com/blog/cns!85EE31844454E642!322.entry)

2\. [避免在cpp源文件中出现静态的中文文字常量](http://zadecn.spaces.live.com/blog/cns%2185EE31844454E642%21323.entry)

3\. [字符集及字符的显示](http://zadecn.spaces.live.com/blog/cns!85EE31844454E642!353.entry)