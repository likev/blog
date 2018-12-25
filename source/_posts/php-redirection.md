---
title: 使用PHP进行HTTP重定向
tags:
  - '301'
  - '302'
  - php
  - 临时
  - 永久
  - 重定向
id: 556
categories:
  - php
  - 文章推荐
date: 2011-02-24 18:32:53
---

在Google里搜“[PHP 重定向](http://www.google.com/search?q=php+重定向)”，[这篇日志](http://yegle.net/2008/03/30/php-redirection/)的排名在第四。但是这篇写得实在太烂了…重写一篇…

## 1. 什么是HTTP重定向？

当你访问www.yegle.net时，地址栏的地址会自动变成yegle.net。当你访问ye.gl的时候，地址栏的地址会变成yegle.net。这就是HTTP重定向

<!-- more -->

一个HTTP请求，返回的HTTP Response Header里，第一行是HTTP的状态码。正常情况下，HTTP请求返回的状态码是200 OK。

正常的HTTP请求，返回200 OK：

```http   

HTTP/1.1 200 OK

Date: Fri, 16 Jul 2010 11:21:10 GMT

Server: Apache

X-Powered-By: PHP/5.2.4-2ubuntu5.10

Set-Cookie: PHPSESSID=7f86ed2e5a4750275e98971773ac88ab; path=/

Expires: Thu, 19 Nov 1981 08:52:00 GMT

Cache-Control: no-store, no-cache, must-revalidate, post-check=0, pre-check=0

Pragma: no-cache

Set-Cookie: wassup=ZjVjMWExMjZjNmIxNzU1NDBhZjU0MmM5MzhmYjllZDQ; expires=Fri, 16-Jul-2010 12:11:11 GMT; path=/

X-Pingback: http://yegle.net/xmlrpc.php

Vary: Accept-Encoding

Transfer-Encoding: chunked

Content-Type: text/html; charset=UTF-8

```

其他常见的返回码如：

```http
    * 404 Not Found
    * 301 Moved Permanently
    * 302 Found
    * 500 Internal Server Error
```

HTTP重定向就是通过301和302两种状态码来实现的。

302是临时重定向的意思。表示被访问页面因为各种需要被临时跳转到其他页面。具体的例子是访问 http://yegle.net/recursion.php

```http

HTTP/1.1 302 Found

Date: Fri, 16 Jul 2010 11:26:48 GMT

Server: Apache

X-Powered-By: PHP/5.2.4-2ubuntu5.10

Location: http://yegle.net/recursion.php

Cache-Control: max-age=600

Expires: Fri, 16 Jul 2010 11:36:48 GMT

Vary: Accept-Encoding

Content-Length: 0

Content-Type: text/html

```

浏览器在收到302 Found的状态码之后会在返回的HTTP Response Header中查找Location字段，然后访问对应地址。在这个例子中，浏览器就会访问 http://yegle.net/recursion.php (嗯这是一个递归，你懂的…)

301是永久重定向。这样的例子很好找。例如 http://google.com

```http
HTTP/1.1 301 Moved Permanently

Location: http://www.google.com/

Content-Type: text/html; charset=UTF-8

Date: Fri, 16 Jul 2010 11:29:07 GMT

Expires: Sun, 15 Aug 2010 11:29:07 GMT

Cache-Control: public, max-age=2592000

Server: gws

Content-Length: 219

X-XSS-Protection: 1; mode=block

```
同样，浏览器在发现301的状态码之后会查找Location字段，然后访问那个地址。

Location字段的格式很随意，既可以是绝对地址，也可以是相对地址，还可以是相对根目录的地址。以下Location字段都是合法的：

```http
Location: http://yegle.net/

Location: /test/index.php

Location: index.php

Location: ../index.php
```
301重定向和302重定向在SEO以及缓存上是有非常大区别的。

对于SEO也就是搜索引擎优化，一个页面302重定向到另一个页面，新页面的PageRank不会受原页面影响。而一个页面301重定向到另一个页面，原页面的PageRank会被传递到新页面。所以对于一个网站进行域名转换，最好的方法就是使用301重定向，在经过一段时间之后可以不损失PR地将全站转移到新域名下。

对于HTTP代理服务器例如squid来说，如果一个页面是302重定向到新页面并且没有指定Expire HTTP头，squid将不缓存这个信息，也就是说每次用户通过代理请求时都会重新获取一遍。而对于301重定向，squid可以将结果缓存以便快速响应下一个请求相同页面的用户。

## 2. 如何用 PHP 实现 301 和 302 重定向？

PHP里的302重定向非常简单，只要在返回的HTTP Response Header里添加Location字段，PHP将自动返回302状态码。例如：

```php
header("Location: http://yegle.net/recursion.php");
```
这段代码将自动重定向到http://yegle.net/recursion.php

而301重定向则稍微有点复杂，需要直接将301状态码用header函数返回给用户。例如：

```php
header( "HTTP/1.1 301 Moved Permanently" );
header( "Location: http://yegle.net/" );
```

注意的是，跳转不是在收到response header的时候马上进行，也就是说页面的剩余内容会被下载来之后浏览器才会跳转。新手常犯的一个错误是，在逻辑判断时对符合条件的情况进行header跳转之后，忘了在之后加上exit()，导致错误。例如，用user_login()判断用户是否进行了登录，如果未登录则跳转到登录页面。代码如下：

```php
if(!user_login()){
    header("Location:login.php");
}
//display contents for login users.
```
这里，容易误以为header返回之后代码就结束了，没有在header之后使用exit()。后面的代码将继续执行，导致未登录用户看到了已登录用户才能看到的内容。
