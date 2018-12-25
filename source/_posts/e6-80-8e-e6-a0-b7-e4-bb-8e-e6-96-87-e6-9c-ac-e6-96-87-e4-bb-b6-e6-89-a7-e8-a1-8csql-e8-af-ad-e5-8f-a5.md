---
title: ' 怎样从文本文件执行SQL语句'
tags:
  - mysql
  - 执行
  - 批处理
  - 文本
  - 查询
  - 语句
id: 752
categories:
  - mysql
date: 2011-08-20 13:01:56
---

mysql客户程序一般交互使用：

shell> mysql db_name

如果你需要在命令行上指定连接参数，命令应为：

shell> mysql -h host -u user -p < batch-file

Enter password: ********

还可以将SQL语句放到一个文件中然后告诉mysql从该文件读取输入。要想实现，创建一个文本文件text_file，并包含你想要执行的语句。然后按如下所示调用mysql：
<pre lang='mysql'>
shell> mysql db_name < text_file
</pre>
还可以用一个USE db_name语句启动文本文件。在这种情况下，不需要在命令行中指定数据库名：
<pre lang='mysql'>
shell> mysql < text_file
</pre>
如果正运行mysql，可以使用source或\.命令执行SQL脚本文件：
<pre lang='mysql'>
mysql> source filename

mysql> \. filename
</pre>
有时想要使用脚本来向用户显示进度信息；为此可以插入下述行：
<pre lang='mysql'>
SELECT '<info_to_display>' AS ' '；
</pre>
将输出<info_to_display>。

如果你有一个产生多个输出的查询，你可以通过一个分页器而不是盯着它翻屏到屏幕的顶端来运行输出：
<pre lang='mysql'>
             shell> mysql < batch-file | more

//你可以捕捉文件中的输出以便进行进一步的处理：

             shell> mysql < batch-file > mysql.out
</pre>
原文链接：[client-side-scripts.html#batch-commands](http://dev.mysql.com/doc/refman/5.1/zh/client-side-scripts.html#batch-commands)