---
title: Ubuntu11.10环境下安装NCL过程记录
tags:
  - ncl
  - 安装
id: 901
categories:
  - NCL
date: 2011-10-21 16:03:37
---

1.NCL软件的介绍和下载见此文：[grow.sinaapp.com/?p=895](http://grow.sinaapp.com/?p=895)

2.安装过程
   此程序无需安装，将下载的ncl_ncarg-6.0.0.Linux_Debian_i686_nodap_gcc445.tar.gz文件解压到任意目录，下面以/usr/local/soft/ncl/ 目录为例说明

   解压后有三个文件夹bin、include和lib，执行程序位于bin目录。
[![ncl-wenjianjia](http://grow-wordpress.stor.sinaapp.com/uploads/2011/10/ncl-wenjianjia.png "ncl文件夹结构")](http://grow-wordpress.stor.sinaapp.com/uploads/2011/10/ncl-wenjianjia.png)
3.设置环境变量
   在终端输入下面的命令打开环境变量文件：
<pre lang='bash'>
sudo gedit /etc/environment
</pre>

编辑文件以添加PATH路径 /usr/local/soft/ncl/bin 和新环境变量NCARG_ROOT="/usr/local/soft/ncl/"，编辑后的文件如下所示：
<pre lang='ini'>
PATH="/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/soft/ncl/bin"
NCARG_ROOT="/usr/local/soft/ncl/"
</pre>

4.测试是否安装成功
在终端输入下面的命令测试是否成功
<pre lang='bash'>
ng4ex gsun01n
</pre>

如果执行成功则会显示下面的绘图界面:
[![配置前的图片](http://grow-wordpress.stor.sinaapp.com/uploads/2011/10/before-peizhi.png "before-peizhi")](http://grow-wordpress.stor.sinaapp.com/uploads/2011/10/before-peizhi.png)

5.修改默认绘图显示方式
在用户主目录里放置一个名称为 .hluresfile 的文件，文件内容示例：[.hluresfile](http://www.ncl.ucar.edu/Document/Graphics/hluresfile)
此时再次运行上面的命令，显示的绘图界面如下：
[![修改配置后的文件](http://grow-wordpress.stor.sinaapp.com/uploads/2011/10/after-peizhi.png "after-peizhi")](http://grow-wordpress.stor.sinaapp.com/uploads/2011/10/after-peizhi.png)