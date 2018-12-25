---
title: 必应(cn.bing.com)首页背景图片调用接口
tags:
  - bing
  - 必应
  - 背景图
id: 1283
categories:
  - html
date: 2013-01-09 17:32:19
---

做了一个简单的API，可调用必应首页背景图片。
使用方法非常简单，只需将图片地址指向 [http://area.sinaapp.com/bingImg](http://area.sinaapp.com/bingImg "http://area.sinaapp.com/bingImg") 即可。
使用下面的CSS代码可以让自己的网页背景图片每天自动更换

```css
body {
    background-image: url("http://area.sinaapp.com/bingImg");
}
```

<!-- more -->

可使用daysAgo参数调用之前的图片，[http://area.sinaapp.com/bingImg?daysAgo=2](http://area.sinaapp.com/bingImg?daysAgo=2 "http://area.sinaapp.com/bingImg?daysAgo=2") 将调用2天前的背景图。
