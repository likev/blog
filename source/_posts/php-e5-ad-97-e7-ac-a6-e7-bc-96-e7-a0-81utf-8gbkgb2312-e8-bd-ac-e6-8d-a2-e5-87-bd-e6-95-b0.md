---
title: 'php 字符编码(utf-8,gbk,gb2312)转换函数'
tags:
  - gb2312
  - gbk
  - php
  - utf-8
  - 函数
  - 编码
  - 转换
id: 791
categories:
  - php
date: 2011-08-21 16:40:46
---

### php中有两个函数可以完成字符编码的转换

#### 1\. iconv函数

函数原型：string iconv ( string $in_charset , string $out_charset , string $str )
说明：此函数为php默认支持的，不需要安装其他模块，而且速度较快，推荐使用。
一些问题：当字符串中包含中文字符**——**(中文输入法下 shift+减号键)时此函数会舍弃此符号及之后的字符

#### 2\. mb_convert_encoding函数

函数原型：string mb_convert_encoding ( string $str , string $to_encoding [, mixed $from_encoding ] )
说明：此函数需要启用 mbstring 扩展库( 在 php.ini里将 ;extension=php_mbstring.dll  前面的 ; 去掉)
一些问题：当php文件自身编码为UTF-8(含BOM)时，转换后的字符串开头有错误的字符。所以php文件一定要以UTF-8(无BOM)格式编码

示例：将字符串从UTF-8编码转换为GB2312编码
<pre lang="php">
header("Content-type: text/html; charset=gb2312");

$str = "abcde 今天是个好天气";

echo mb_convert_encoding($str,"gb2312","UTF-8");

echo '
';

echo iconv("UTF-8", "gb2312", $str);
</pre>