---
title: matlab基础回顾
tags:
  - MATLAB
  - 矩阵
  - 绘图
id: 368
categories:
  - matlab
date: 2011-01-04 15:39:26
---

*   ## 向matlab中输入矩阵（matrices）的几种方式

    1.  ### 手动输入

格式：

            *   1.用空白或者逗号（commas）分隔元素
        *   2.用分号（semicolon）分隔每一行
        *   3.用方括号包围整个元素列表
如 A = [16 3 2 13; 5 10 11 8; 9 6 7 12; 4 15 14 1]
    2.  ### 函数生成（包括内置和用户自定义函数）

内置函数如：zeros magic ones rand randn 另外还可以用 A=a:s:b 的方式生成从a到b，间隔为s的矩阵。比如A=2:2:6 执行后A
= [2,4,6],当s为1时可简写为A=a:b

	<!--more-->3.  ### 从文件导入

            *   1.从文本文件（包括csv格式）导入 csvread/csvwrite dlmread/dlmwrite textread textscan
        *   2.从mat文件导入 load/save
        *   3.从excel或者lotus123 表格（Spreadsheets）导入 xlsfinfo xlsread/xlswrite wk1read/wk1write
        *   4.从xml文件导入 xslt xmlread/xmlwrite
        *   5.直接文件读取 fopen/fclose fread/fscanf/fwrite/fprintf/fgets/fgetl/ftell/fseek/feof
        *   6.从网络读取 urlread/urlwrite/ftp/sendmail zip/unzip
        *   7.科学数据读取 cdfinfo/cdfread/cdfwrite
        *   8.音视频和图片文件读取 imread/imwrite/imfinfo

*   ## matlab中矩阵的处理

    *   ### 1.基本运算

1.表达式 + - * / .* ./ ' 2.函数 求和sum 转置',
    *   ### 2.子矩阵操作

            *   1.A(a:b) 提取第a到b个元素，按每一列计数，生成一个行向量 A(2:2:10) 提取第2,4,6,8,10个元素
        *   2.A(a:b,c:d) 提取从a到b行，从c到d列的数据。 提取所有行的数据 A(:,c:d) 提取最后一列的数据 A(a:b,end) 提取偶数行 A(2:2:end,:)
        *   3.将第一行和第三行交换 B=A([3 2 1],:)
        *   4\. 生成更大的矩阵 B = [A A+32; A+48 A+16]
        *   5\. 删除列 A[:,3] = []

*   ## matlab中简单的绘图

    *   1.基本函数 box plot/plot3/plotyy loglog polar subplot fplot
    *   2.等值线函数 contour/contour3 contourc contourf
    *   3.其他函数 area bar/bar3/bar3h pie/pie3
<div>

## 其他资源

1\. matlab官方入门视频  [getting-started-with-matlab](http://www.mathworks.cn/videos/getting-started-with-matlab-68985.html?s_tid=main_tutorial_ML_rp "getting-started-with-matlab")
2\. matlab在线手册 [help/matlab](http://www.mathworks.cn/cn/help/matlab/index.html "help/matlab")
</div>