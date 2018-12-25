---
title: 在XP及Ubuntu上快速安装及配置LAMP(Linux+Apache+Mysql+Php/Perl/Python)环境
tags:
  - apache
  - PATH
  - php
  - xp
  - 加载
  - 安装
  - 服务器
  - 模块
  - 环境
  - 配置
id: 85
categories:
  - php
  - 互联网
  - 记录
date: 2011-08-10 06:36:48
---

## Ubuntu 快速安装LAMP环境及配置方法：

#### 一 安装LAMP环境
在终端输入以下命令(是的，你没看错，只用一条命令即可)

```cmd
sudo apt-get install apache2 mysql-server mysql-client php5 php5-gd php5-mysql
```
安装过程中会要求你设置MySQL的帐户root密码，暂时可以直接回车，不设置密码

#### 二 配置LAMP环境
Apache2默认安装在/etc/apache2目录下
打开用户配置文件：

```cmd
sudo gedit /etc/apache2/httpd.conf
```

添加下面的一行来启用php文件类型支持：

```apache
AddType application/x-httpd-php .php .php5
```

至此LAMP已可以正常运行 网站目录默认在 /var/www

#### 三 其他可选配置

    1. apache 的配置文件路径 /etc/apache2/httpd.conf
    2. php.ini 路径 /etc/php5/apache2/php.ini
    3. mysql配置文件 路径 /etc/mysql/my.cnf
    4. phpmyadmin配置文件路径 /etc/phpmyadmin/apache.conf
    5. 网站根目录配置文件路径 /etc/apache2/sites-enabled



## XP 快速安装LAMP环境及配置方法：

#### 一 安装及配置Apache

1. 打开网页 选择合适的版本下载
http://httpd.apache.org/download.cgi

2. xp下双击安装包，直接安装
ubuntu下安装说明见 [apache.org/docs/2.2/install.html](http://httpd.apache.org/docs/2.2/install.html)

3. 打开conf/httpd.conf  进行配置

    ```apache
    #配置网站所在的文件夹
    DocumentRoot "D:/webdocs"
    ```
    ```apache
    #配置网站文件夹的属性
    <Directory "D:/webdocs">

       #当文件不存在时不要列出目录中的文件列表
        Options -Indexes FollowSymLinks

        #
        # AllowOverride controls what directives may be placed in .htaccess files.
        # It can be "All", "None", or any combination of the keywords:
        #   Options FileInfo AuthConfig Limit
        #
        AllowOverride None

        #
        # 控制对此目录的访问权限
        #
        Order allow,deny
        Allow from all

    </Directory>
    ```

#### 二 安装及配置Mysql
Ubuntu下安装过程见此文 [ubuntu 10.04 MySQL 5.5.11 源代码编译安装](http://forum.ubuntu.org.cn/viewtopic.php?t=330121)
XP下可直接下载安装包

#### 三 安装及配置PHP

1. 下载 the PHP zip binary distribution from [» PHP for Windows: Binaries and Sources](http://windows.php.net/download/).

    选择 VC6 x86 Thread Safe 版本

2. 直接解压后放在softs文件夹下即可

3. 在安装目录中另存 php.ini-production 为 php.ini 并进行配置

    a.设置模块目录并开启需要的模块

    ```ini
    ; Directory in which the loadable extensions (modules) reside.
    ; 此项设置模块所在的目录，注意如果path变量没有设置php安装目录时
    ; 此项一定要设置为绝对目录，否则Apache将无法正确加载php扩展模块
    extension_dir = "D:/softs/php-5.2.17/ext/"
    ```

    以上设置不正确时将会出现类似下述错误信息
    ```
    PHP Warning:  PHP Startup: Unable to load dynamic library './ext/php_bz2.dll' - \xd5\xd2\xb2\xbb\xb5\xbd\xd6\xb8\xb6\xa8\xb5\xc4\xc4\xa3\xbf\xe9\xa1\xa3\r\n in Unknown on line 0
    PHP Warning:  PHP Startup: Unable to load dynamic library './ext/php_curl.dll' - \xd5\xd2\xb2\xbb\xb5\xbd\xd6\xb8\xb6\xa8\xb5\xc4\xc4\xa3\xbf\xe9\xa1\xa3\r\n in Unknown on line 0
    ```

     b.设置可最大上传文件的大小和默认时区等选项
    ```
    [Date]
    ; Defines the default timezone used by the date functions
    date.timezone = Asia/Chongqing
    ```

4. 打开apache 的 conf/httpd.conf  进行配置

    ```apache
    # 让apache自动在每次启动时加载php模块. apache2.2 版本需要加载php5apache2_2.dll
    LoadModule php5_module "D:/softs/php-5.2.17/php5apache2_2.dll"
    AddHandler application/x-httpd-php .php

    # 配置 php.ini 文件所在路径
    PHPIniDir "D:/softs/php-5.2.17"
    ```

5. 重启计算机

---

今天调试网页时发现apache服务器经常自动重启，打开error.log文件后发现下述信息

[Sat Aug 20 19:43:25 2011] [notice] Parent: child process exited with status **3221225477** -- Restarting

在网上查找一番后发现原因是php文件中包含了数据库查询语句，而apache调用了与当前版本不一致的**libmysql.dll** 所致。
由于安装的mysql 数据库是早期版本，在安装mysql后程序自动设定**mysql安装目录**为**PATH**环境变量。mysql安装目录下含有版本不一致的libmysql.dll 文件，apache调用了那个不合适的文件后产生错误。

而在安装php时并没有将php目录设定为PATH环境变量。

**解决办法：** 删除mysql安装目录里面的libmysql.dll 文件，然后将php安装目录设置为PATH环境变量即可。
