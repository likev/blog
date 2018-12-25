---
title: php 用header下载文件
tags:
  - header
  - php
  - 下载
  - 代码
  - 文件
id: 667
categories:
  - php
  - 互联网
  - 编程
date: 2011-08-12 17:49:51
---

你希望客户要填完一份表格，然后就将网址指到该文件，这样客户才能下载，但如果你想做一个关于"网上购物"的电子商务网站，考虑安全问题，你不想用户直接复制网址下载该文件，笔者建议你使用PHP直接读取该实际文件然后下载的方法去做。程序如下：

一 下载当前服务器文件

<pre lang="php">
$file_name = "info_check.exe";
$file_dir = "/public/www/download/";
if (!file_exists($file_dir . $file_name)) { //检查文件是否存在
echo "文件找不到";
exit;
} else {
$file = fopen($file_dir . $file_name,"r"); // 打开文件
// 输入文件标签
Header("Content-type: application/octet-stream");
Header("Accept-Ranges: bytes");
Header("Accept-Length: ".filesize($file_dir . $file_name));
Header("Content-Disposition: attachment; filename=" . $file_name);
// 输出文件内容
echo fread($file,filesize($file_dir . $file_name));
fclose($file);
exit;}
</pre>

二 下载远程文件
而如果文件路径是"http" 或者 "ftp" 网址的话，则源代码会有少许改变，程序如下：
<pre lang="php">
$file_name = "info_check.exe";
$file_dir = "http://www.easycn.net/";
$file = @ fopen($file_dir . $file_name,"r");
if (!$file) {
echo "文件找不到";
} else {
Header("Content-type: application/octet-stream");
Header("Content-Disposition: attachment; filename=" . $file_name);
while (!feof ($file)) {
echo fread($file,50000);
}
fclose ($file);
}
</pre>

这样就可以用PHP直接输出文件了。

三 一般情况只需要三条语句即可
<pre lang="php">
header ('Content-type: application/'.$file_ext);
header ("Expires: 0");//可选
header ("Pragma: no-cache"); //可选
header ('Content-Disposition: attachment; filename='.$file_name.'');
header ("Content-Length: ".$file_size);  //可选
readfile ($file_name);
</pre>

原文链接：[http://lhdeyx.blog.163.com/.../31819697200983010224884/](http://lhdeyx.blog.163.com/blog/static/31819697200983010224884/)