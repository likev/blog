---
title: 'jQuery 1.9版, jQuery 2.0 beta版, jQuery Migrate插件1.0发布'
tags:
  - jquery
  - jQuery 1.9
id: 1289
categories:
  - html
  - javascript
date: 2013-01-16 08:46:28
---

### 一、几点说明

*   jQuery 1.9 和 2.0版 拥有相同的API，这两个版本将**长期同时**存在，2.0版本不再支持Internet Explorer 6, 7, and 8 (“oldIE”)
*   jQuery 1.9 和 2.0版移除了一些过时的API(在之前版本中被标记为deprecation)，从而可以使jQuery更稳定和高效，如果你的代码中使用了一些过时的API，你可以使用jQuery Migrate插件恢复移除的API

```javascript
<script src="http://code.jquery.com/jquery-1.9.0.js"></script>
<script src="http://code.jquery.com/jquery-migrate-1.0.0.js"></script>
```

### 二、移除的函数有：

*   .toggle(function, function, ... ) 请不要和切换显隐的.toggle()函数混淆，后者没有被移除
*   jQuery.browser() 如果需要请使用[jQuery.browser](https://github.com/jquery/jquery-browser "https://github.com/jquery/jquery-browser")插件*   .live() 请使用.on()方法替代
*   .die() 请使用.off()方法替代
*   jQuery.sub()

其他说明请参考官方文档

*   [jQuery 1.9 final, jQuery 2.0 beta, Migrate final released(发布说明)](http://blog.jquery.com/2013/01/15/jquery-1-9-final-jquery-2-0-beta-migrate-final-released/ "http://blog.jquery.com/2013/01/15/jquery-1-9-final-jquery-2-0-beta-migrate-final-released/")*   [jQuery Core 1.9 Upgrade Guide(升级说明)](http://jquery.com/upgrade-guide/1.9/ "http://jquery.com/upgrade-guide/1.9/")