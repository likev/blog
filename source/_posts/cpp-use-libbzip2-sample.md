---
title: C++使用libbzip2解压文件代码示例
id: 1327
categories:
  - C++
date: 2014-07-05 20:02:56
tags:
---

bzip2的最新版本是 1.0.6, 发布于 20 Sept 2010\. 也就是说将近4年没更新了，在这个计算机技术日新月异的时代，其代码已稍许陈旧。
使用Visual Studio Express 2013编译libbzip2库时有好几个安全提示，比如fopen需改为fopen_s(其实微软也相当蛋疼，可使用#define _CRT_SECURE_NO_WARNINGS 关闭错误提示)

libbzip2库的相关介绍和代码示例相当少，除了官方不那么清晰的文档我用Google几乎没找到其他示例。它提供了高级和低级两类API，其中高级API解压函数BZ2_bzRead死活不能编译通过，只好用所谓的低级API BZ2_bzDecompress(其实使用还相当方便)。

下面这些简短代码花费了我一整天的时间，放上来与大家分享。

```cpp
#include <iostream>
#include <fstream>
#include <string>

#include "bzlib.h"

int use_low_level_interface()
{
	//定义两个字符串分别用来存储压缩字符流 和 输出字符流
	std::string instr(200,' '), outstr;
	//instr = std::string(100, 'a') + std::string(100, 'b');

	//将压缩文件读入instr 压缩前原文件包含100个a和100个b
	std::ifstream fin("100ab.txt.bz2", std::ios_base::in | std::ios_base::binary);
	fin.read(&*instr.begin(), instr.size());

	instr.resize(fin.gcount());
	std::cout <<"压缩后字符串:"<<instr;

	fin.close();

	outstr.resize(1000);

	//bz_stream 数据结构用来存储压缩流和解压流相关信息
	bz_stream bsread;
	bsread.bzalloc = NULL;
	bsread.bzfree = NULL;
	bsread.opaque = NULL;

	//初始化bsread 比如设置总输入和输出长度为0 设置压缩状态 
	//第二个参数设置解压状态输出 设为0不输出内部状态
	BZ2_bzDecompressInit(&bsread, 4, 0);

	int ret, last_total_out=0;

	//设置输入输出位置和字节数
	bsread.avail_in = instr.size();
	bsread.next_in = &*instr.begin();

	bsread.avail_out = 70;//outstr.size()
	bsread.next_out = &*outstr.begin();	

	do{//循环解压 每次解压最多70字节存入outstr并输出

	ret = BZ2_bzDecompress(&bsread);

	std::cout << "\n bsread.total_out_hi32:" << bsread.total_out_hi32
		<< "\n bsread.total_out_lo32:" << bsread.total_out_lo32;
	std::cout << " ret:" << ret;

	std::cout << '\n' << outstr.substr(0, bsread.total_out_lo32 - last_total_out);

	last_total_out = bsread.total_out_lo32;

	//BZ2_bzDecompress函数每次执行后自动设置avail_in next_in avail_out next_out
	//比如第一次执行到此位置时 avail_in==10 avail_out=0 
	bsread.avail_out = 70;
	bsread.next_out = &(*outstr.begin() );

	} while (ret == BZ_OK);

	BZ2_bzDecompressEnd(&bsread);

	return 0;
}

int main()
{
	use_low_level_interface();

	return 0;
}
```

上述程序输出结果如下：
<pre>
压缩后字符串:BZh91AY&SY噦
    [1: huff+mtf rt+rld
 bsread.total_out_hi32:0
 bsread.total_out_lo32:70 ret:0
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
 bsread.total_out_hi32:0
 bsread.total_out_lo32:140 ret:0
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaabbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb {0xa45487
82, 0xa4548782}]
    combined CRCs: stored = 0xa4548782, computed = 0xa4548782
 bsread.total_out_hi32:0
 bsread.total_out_lo32:200 ret:4
bbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb请按任意键继续. . .
</pre>

测试数据下载:[100ab.txt.bz2](http://grow-wordpress.stor.sinaapp.com/uploads/2014/07/100ab.txt.bz2)