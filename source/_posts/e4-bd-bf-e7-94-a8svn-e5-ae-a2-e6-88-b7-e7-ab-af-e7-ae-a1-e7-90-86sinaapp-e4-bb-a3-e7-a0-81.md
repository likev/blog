---
title: SVN命令行客户端安装与配置(管理sinaapp代码)
tags:
  - svn
  - 安装
  - 客户端
  - 配置
id: 35
categories:
  - 编程
  - 记录
date: 2011-08-09 12:48:50
---

1.下载命令行客户端

http://www.collab.net/downloads/subversion/
下载地址：[1.官网下载 需登录](http://www.open.collab.net/files/documents/60/4635/CollabNetSubversion-client-1.6.17-4.win32.exe)
[2.dbank网盘下载](http://dl.dbank.com/c0blnmlm5u)

2.安装及配置

双击安装
配置文件所在路径 
XP: C:\Documents and Settings\your-username\Application Data\Subversion
Win7: C:\Users\your-username\AppData\Roaming\Subversion

打开server文件进行HTTP代理配置(如果没有使用代理可跳过这一步)
<pre lang='ini' line='142'>
[global]
# http-proxy-exceptions = *.exception.com...
http-proxy-host = 172.18.172.251
http-proxy-port = 80
</pre>

3.部署代码

http://sae.sina.com.cn/?m=devcenter&amp;catId=212