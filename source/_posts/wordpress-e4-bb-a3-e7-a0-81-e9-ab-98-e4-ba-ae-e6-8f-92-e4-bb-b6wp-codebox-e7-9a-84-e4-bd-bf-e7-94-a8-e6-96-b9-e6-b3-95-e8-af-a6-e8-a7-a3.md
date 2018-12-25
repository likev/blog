---
title: wordpress代码高亮插件wp-codebox的使用方法详解
tags:
  - 代码
  - 使用
  - 插件
  - 示例
  - 语言
  - 高亮
id: 768
categories:
  - wordpress
date: 2011-08-21 01:29:49
---

使用说明

&lt;pre lang="LANGUAGE" line="1" file="download.txt" colla="+"&gt;
//这里写你的代码
&lt;/pre&gt;

可用参数:
* lang="LANGUAGE" -    所用的语言
* file="download.txt" -  将创建一个下载链接.
* line="N"  - 开始行号.
* colla="+/-"   - The `+/-` 将打开/折叠 codebox.
* line,file,colla是可选的.

lang参数常用的值如下

c cpp php css javascript html4strict xml python perl reg mysql matlab ini java bash dos asp actionscript

示例代码1

&lt;pre lang='cpp'&gt;
#include &lt;iostream&gt;

int main()
{
int a=3;
double b=12.8;
char * m = "a string";

std::cout&lt;&lt;"a = "&lt;&lt;a&lt;&lt;"  b = "&lt;&lt;b&lt;&lt;"   m = "&lt;&lt;m&lt;&lt;std::endl;
}
&lt;/pre&gt;

将产生如下输出
<pre lang="cpp">
#include <iostream>

int main()
{
	int a=3;
	double b=12.8;
	char * m = "a string";

	std::cout<<"a = "<<a<<"  b = "<<b<<"   m = "<<m<<std::endl;
}
</pre>