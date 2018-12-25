---
title: 支持通配符和正则表达式的hosts文件(本地dns缓存及代理)
date: 2014-11-22 18:47:50
---
## hosts文件存在的问题
windows下的hosts文件可用来指定网址到ip的映射，而不用通过DNS服务器解析。某些情况下这是非常有用的，比如可防止某些域名被DNS污染，可加速常用网站的DNS查询，可屏蔽网站中大量的广告，但是windows自带的hosts文件功能较弱，编辑起来非常麻烦，不支持通配符，如果一个网站有大量二级或三级子域名，需要在hosts文件添加大量记录，如果这些子域名对应的ip改变，需要对大量记录进行修改，维护起来非常麻烦且容易出错。

## 解决方案
有没有一个软件可以解决上面提到的问题？
今天要介绍的是 Acrylic([官网地址](http://mayakron.altervista.org/wikibase/show.php?id=AcrylicHome "官方网站") / [开源项目地址](http://sourceforge.net/projects/acrylic/ "项目地址"))。

Acrylic是一个本地DNS代理，比如以前你设置dns为8.8.8.8,现在你只需设置本机dns为127.0.0.1即可，然后配置Acrylic使用8.8.8.8。当你请求taobao.com时，Acrylic使用8.8.8.8解析taobao.com的ip，然后将这个ip缓存起来，下次再访问taobao.com时就从缓存中读取ip。

聪明的你可能知道windows本身是具有dns缓存功能的，各大浏览器也具有DNS缓存或DNS预解析功能，所以这不是本文章的重点。

<!-- more -->
## 安装与配置
先说一下安装，Acrylic使用Borland Delphi编写，只支持windows，可从官网下载安装文件，安装文件只有400KB，非常小巧。安装过程非常简单不再赘述。

安装完以后Acrylic会以windows服务的方式启动，默认Acrylic使用OpenDNS的地址208.67.222.222来解析，你也可手动修改安装目录下的AcrylicConfiguration.ini配置文件中的PrimaryServerAddress选项来修改为你想使用的DNS服务，比如google的8.8.8.8或阿里的223.5.5.5。

Acrylic安装目录下的AcrylicHosts.txt文件为Acrylic使用的Hosts文件，支持通配符*(匹配0或多个字符)和?(匹配0或一个字符)。并且支持一个ip对应多个地址。
比如下面这行代码将baidu的主域名和子域名全部解析到119.161.83.30这个地址。
<pre lang='hosts'>
 119.161.83.30 *.baidu.com baidu.com
</pre>

AcrylicHosts.txt还支持正则表达式(以反斜杠开头的地址被当做正则表达式处理)，比如下面这行代码同样将baidu的主域名和子域名全部解析到119.161.83.30这个地址。
<pre lang='hosts'>
 119.161.83.30 /(\S+\.)?baidu.com
</pre>

AcrylicHosts.txt还支持在通配符中排除指定子域名，比如下面这行代码将除pan.baidu.com之外的所有baidu的子域名解析到119.161.83.30这个地址。
<pre lang='hosts'>
 119.161.83.30 *.baidu.com baidu.com -pan.baidu.com
</pre>

修改AcrylicHosts.txt之后记得清除Acrylic缓存并重启Acrylic服务，可通过开始菜单清除，或cmd-->cd C:\Program Files\Acrylic DNS Proxy-->AcrylicController.exe PurgeAcrylicCache

另外一定要记得将网络的DNS设置为127.0.0.1 
[![DNS设置](http://grow-wordpress.stor.sinaapp.com/uploads/2014/11/127.jpg)](http://grow-wordpress.stor.sinaapp.com/uploads/2014/11/127.jpg)

在单位电脑做好以上配置后，是否可以让单位其他电脑共享你的配置呢，当然可以，Acrylic本来就是一个DNS代理。假设你的电脑IP为192.168.0.3，只需在其他电脑上将DNS配置为192.168.0.3即可。相当于一个单位内部DNS服务器。

AcrylicConfiguration.ini配置文件中还有一些其他的有用选项，比如控制哪些域名不进行缓存([CacheExceptionsSection]选项)，控制哪些电脑可以访问本DNS服务([AllowedAddressesSection]选项)。
