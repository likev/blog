---
title: C++ 读取整个文件，每行有不确定的数
id: 215
categories:
  - C++
date: 2009-12-18 09:58:49
tags:
---

double val=0;

vector&lt;double&gt; vecdle;

string sline;

ifstream fin("filename")

while(getline(fin,sline))

{

istringstream ssin(sline);
<p style="padding-left: 30px;">while(ssin&gt;&gt;val)
{
vecdle.push_back(val);
}

}[
](http://www.google.cn/webhp?source=g_cn)