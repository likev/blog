---
title: php字符串中单引号和双引号的区别
tags:
  - php
  - 区别
  - 单引号
  - 双引号
  - 字符串
  - 规则
  - 转义
id: 780
categories:
  - php
date: 2011-08-21 11:22:51
---

在php中可以用单引号或者双引号来表示一个字符串：

<pre lang='php'>
$str1 = 'this is a string';
$str2 = "this is a string";
</pre>
以上的两个字符串是相同的 $str1 = $str2 = **this is a string**

但是两种表示方法在一些情况下是不同的
<pre lang='php'>
$str1 = 'a\nb\\c\$dd\t\'\"dfeee\x30mmm';
echo $str1;
$str2 = "a\nb\\c\$dd\t\'\"dfeee\x30mmm";
echo $str2;
</pre>

str1将输出以下代码
<pre>
a\nb\c\$dd\t'\"dfeee\x30mmm
</pre>

str2将输出以下代码
<pre>
a
b\c$dd	\'"dfeee0mmm
</pre>

在单引号表示的字符串中，只有**\'**和**\\**会被进行转义
在双引号表示的字符串中，以下情况将被转义
<table class="doctable table">
<thead valign="middle">
      <tr valign="middle">
       <th>表示法</th>
       <th>含义</th>
      </tr>

     </thead>

     <tbody valign="middle" class="tbody">
      <tr valign="middle">
       <td align="left">_\n_</td>
       <td align="left">换行 (LF or 0x0A (10) in ASCII)</td>
      </tr>

      <tr valign="middle">
       <td align="left">_\r_</td>
       <td align="left">回车 (CR or 0x0D (13) in ASCII)</td>
      </tr>

      <tr valign="middle">
       <td align="left">_\t_</td>
       <td align="left">水平方向的 tab(HT or 0x09 (9) in ASCII)</td>
      </tr>

      <tr valign="middle">
       <td align="left">_\v_</td>
       <td align="left">竖直方向的 tab (VT or 0x0B (11) in ASCII) (since PHP 5.2.5)</td>
      </tr>

      <tr valign="middle">
       <td align="left">_\f_</td>
       <td align="left">换页 (FF or 0x0C (12) in ASCII) (since PHP 5.2.5)</td>
      </tr>

      <tr valign="middle">
       <td align="left">_\\_</td>
       <td align="left">反斜线</td>
      </tr>

      <tr valign="middle">
       <td align="left">_\$_</td>
       <td align="left">美金dollar标记</td>
      </tr>

      <tr valign="middle">
       <td align="left">_\"_</td>
       <td align="left">双引号</td>
      </tr>

      <tr valign="middle">
       <td align="left">_\[0-7]{1,3}_</td>
       <td align="left">
        符合该表达式顺序的字符串是一个八进制的字符
       </td>
      </tr>

      <tr valign="middle">
       <td align="left">_\x[0-9A-Fa-f]{1,2}_</td>
       <td align="left">
        符合该表达式顺序的字符串是一个十六进制的字符
       </td>
      </tr>

     </tbody>

   </table>