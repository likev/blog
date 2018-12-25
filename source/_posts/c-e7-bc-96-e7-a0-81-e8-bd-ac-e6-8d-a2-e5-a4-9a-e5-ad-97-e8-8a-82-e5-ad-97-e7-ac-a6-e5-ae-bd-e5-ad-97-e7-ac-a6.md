---
title: C++ 编码转换 多字节字符 宽字符
tags:
  - C++
  - 编码
id: 221
categories:
  - C++
date: 2010-01-12 09:07:21
---

## <span style="color: #2b3cd3;"> C++ 中可用的字符编码总体上说有两种： 一种为多字节字符， 如Ansi编码，每个汉字由2个char 确定，或者utf-8编码，每个汉字由三个char 确定。另一种为宽字符编码，每个汉字直接由1个short(wchar_t)确定。</span>

## <span style="color: #2b3cd3;">自己利用两个Win32 API函数写了两个用于编码转换的函数</span>

<pre lang='cpp'>
//编码转换

#include <string>

#include <Windows.h>

//UTF8编码转换为Ansi编码
std::string & Utf8ToAnsi(std::string &scr, std::string &des)
{
	size_t n = scr.size()*2;
	wchar_t *sl = new wchar_t[n];

	char *sm = new char[n];
	//多字节(UTF8)编码转换为宽字节编码
	MultiByteToWideChar(CP_UTF8,0,scr.c_str(),-1,sl,n);

	//宽字节转换为多字节(Ansi)编码
	WideCharToMultiByte(CP_ACP, 0,sl, -1,sm, n,NULL,0);

	des = sm;
	delete []sl;
	delete []sm;

	return des;
}

//Ansi编码转换为Unicode(Utf16)编码
std::wstring & AnsiToUtf16(std::string &scr, std::wstring &des)
{
	size_t n = scr.size();

	wchar_t *sl = new wchar_t[n+1];

	MultiByteToWideChar(CP_ACP,0,scr.c_str(),-1,sl,n+1);

	des = sl;
	delete []sl;

	return des;
}
</pre> 