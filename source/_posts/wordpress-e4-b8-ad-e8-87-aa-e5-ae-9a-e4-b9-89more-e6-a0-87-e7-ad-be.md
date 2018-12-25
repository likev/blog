---
title: WordPress中自定义more标签
tags:
  - Ajax
  - more 标签
  - wordpress
id: 429
categories:
  - wordpress
date: 2011-01-06 14:45:05
---

wordpress是十分强大的php语言个人博客系统，安装使用都很方便，可以google一下。
下面简单谈谈more标签的使用。

我们都想在首页显示尽可能多的文章，又不想让页面太长影响用户体验，在合适的位置添加more标签是个不错的主意。
more标签是wordpress的一种html注释方式的标记，如右所示： &lt;!--more--&gt; 要注意字母m之前不能有空格，也就是说&lt;!-- more--&gt; 不是more标签，而是注释。

当添加more标签后，之后的文章内容将不会被显示，而是以一个**指向单独文章的链接**来表示，链接的文本默认为[更多...](http://blog.lyqx.de/?p=429)这样的形式。

下面简单说一下修改链接默认文本的方式，比如从“更多...”改为“阅读更多内容...”

首先进入wordpress后台管理页面，展开 外观(themes) 选项卡，选择 编辑，可以看到右边有很多主题相关的文件，如index.php，page.php，header.php等，每个文件分别对应页面的一个位置。点击index.php(没有这个文件的话点击home.php)，在第20行左右找到类似&lt;?php the_content('更多...'); ?&gt; 这一行，直接修改"更多..."为“阅读更多内容...”即可。
<!--more-->
当然有的主题下面找不到那一行，比如我的主题下面是&lt;?php pp_the_content(); ?&gt;，说明此主题对the_content函数进行了包装，点击functions.php这个文件，找到pp_the_content这个函数，在函数体内将the_content('更多...')修改为the_content('阅读更多内容...')就可以了。

详细的修改方式请参考官方文档[Customizing_the_Read_More](http://codex.wordpress.org/Customizing_the_Read_More)
关于the_content函数的更多介绍也请参考官方文档[the_content](http://codex.wordpress.org/Template_Tags/the_content)

默认情况下点击"更多..."链接时将打开新的窗口来显示单独的一篇文章，我们可以利用插件来改变这个行为，此处向大家推荐 Read More Right Here 这个插件，当点击更多链接时将用Ajax方式在当前页显示更多内容，正如插件名字所示。