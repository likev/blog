---
title: svn 连接 Google Project Hosting
tags:
  - Google
  - Project
  - Subversion
  - svn
  - 代码
  - 控制
  - 版本
  - 项目
id: 604
categories:
  - 编程
date: 2011-04-09 11:22:38
---

初接触svn和google项目托管，在摸索中使用。

### 迁出项目代码方法：

svn checkout https://project-name.googlecode.com/svn/trunk/ local-dir-name --username yourname
其中project-name是你的项目名称
local-dir-name是本地的目录，若不存在则创建，如不指定则默认为trunk
yourname是您的google账户名称

### 本地修改代码后提交至google项目托管的方法：

svn commit --message "log info" local-dir-name
提交时必需用参数 --message提供log信息，信息可以为空
如果当前本地目录为代码所在目录，则不需要指定local-dir-name

执行上述命令后会提示你输入密码
Authentication realm:  &lt;https://project-name.googlecode.com:443&gt; Google Code Subvers
ion Repository
Password for 'yourname': ***

昨天我输入google账户密码时出现了以下信息
svn: Commit failed (details follow):
svn: Server sent unexpected return value (500 Internal Server Error) in response
to MKACTIVITY request for '/svn/!svn/act/a023056f-33d9-4342-a62f-39bf04ea2915'
也就是说提交失败了，上网查说是URL大小写，卡巴斯基阻挡等原因。当我改了大小写并关闭了卡巴斯基后还是提交失败。
今天在网上搜索google项目托管的使用方法才发现原因其实很简单，也就是密码错误。

注意此处的密码为googlecode.com 的密码，也就是你在google托管项目的密码，和google账户的密码是不一样的。
获取密码的方法如下图所示
<table style="width: auto;">
<tbody>
<tr>
<td>[![](https://lh5.googleusercontent.com/_lt9Z389dy-U/TZ_LHWzslmI/AAAAAAAAJ_Q/z-nB3qeKGp0/s400/password.jpg)](https://picasaweb.google.com/lh/photo/sYYer4c8S96NuTRUs5WwCA?feat=embedwebsite)</td>
</tr>
<tr>
<td style="font-family: arial,sans-serif; font-size: 11px; text-align: right;">发件人 [网络图片](https://picasaweb.google.com/117677758756544859666/srBFLL?feat=embedwebsite)</td>
</tr>
</tbody>
</table>
Google Project Hosting 地址：[http://code.google.com/hosting/](http://code.google.com/hosting/)
使用Subversion进行版本控制：[http://svndoc.iusesvn.com/svnbook/1.4/index.html](http://svndoc.iusesvn.com/svnbook/1.4/index.html)
SVN软件：[http://subversion.../packages.html](http://subversion.apache.org/packages.html "SVN软件")