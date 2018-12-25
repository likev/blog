---
title: 字符编码的转换（C++为例）
id: 258
categories:
  - C++
date: 2010-09-17 05:58:24
tags:
---

出处:[http://www.cppblog.com/chemz/archive/2007/05/30/25133.html](http://www.cppblog.com/chemz/archive/2007/05/30/25133.html "http://www.cppblog.com/chemz/archive/2007/05/30/25133.html")

内容如下:

字符集相关问题
字符集目前有两个大的类别：本地字符集和国际字符集，其中每一类别的字符集又有多个
不同的字符编码实例。比如：本地字符集中基本上对于每一个不同的地区和国家就会形成一个
属于自己的字符集（ascii, latin-1, chs等），国际字符集中同样包括多种不同的编码方案
（utf8, utf16等）。
那么在C/C++程序中如何完成上述字符集之间的转换工作呢？分成两种情况：
1\. 通过const char *cstr使用开发环境中的编辑器输入字符串常量"中国"，如下：
const char *cstr = "中国";
这样一来cstr所指向的字符串内存中保存的则是本地字符编码下所形成的字符串，也
就是说，上面的cstr中存储着chs字符编码集中的字符；
2\. 通过const wchar_t *wstr使用开发环境中的编辑器输入字符串常量"中国"，如下：
const wchar_t *wstr = L"中国";
这样一来wstr所指向的字符串内存中保存的则是国际字符编码（在VC++下是ucs2，
在gcc下是ucs4）下所形成的字符串，也就是说，上面的wstr中存储着utf16字符编
码集中的字符；
那么如何将cstr转换成为wstr呢？可以通过C语言中的标准转换函数mbstowcs来完成该工
作，此时需要注意的是如果直接使用mbstowcs进行转换会得到一个错误的结果，并不能成功
的完成转换成为国际宽字符的要求，这是为什么呢？在C/C++语言标准中定义了其运行时的
字符集环境为"C"，也就是ASCII字符集的一个子集，那么mbstowcs在工作时会将cstr中所包
含的字符串看作是ASCII编码的字符，而不认为是一个包含有chs编码的字符串，所以他会将
每一个中文拆成2个ASCII编码进行转换，这样得到的结果就是会形成4个wchar_t的字符组成
的串，那么如何才能够让mbstowcs正常工作呢？在调用mbstowcs进行转换之间必须明确的告
诉mbstowcs目前cstr串中包含的是chs编码的字符串，通过setlocale( LC_ALL, "chs" )函数
调用来完成，需要注意的是这个函数会改变整个应用程序的字符集编码方式，必须要通过重
新调用setlocale( LC_ALL, "C" )函数来还原，这样就可以保证mbstowcs在转换时将cstr中
的串看作是中文串，并且转换成为2个wchar_t字符，而不是4个。