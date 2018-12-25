---
title: wxWidgets 多平台开发心得
tags:
  - 多平台
  - 开发
id: 313
categories:
  - C++
  - wxWidgets
date: 2010-12-27 22:36:15
---

### 不得不承认C++跨平台开发是有一定难度的，即使有wxWidgets这么好的库。

### 首先要考虑文件系统方面的差异：

*   1.Ubuntu下面C++的源代码使用UTF8无BOM格式，换行符为n, 而在XP下面则为ansi编码，换行符为rn,源代码要进行转换。
*   2.Ubuntu下面路径分隔符为/,而xp下面则为, 一定要注意在字符串中此字符表示为"",可以用wxFILE_SEP_PATH宏统一起来

## 其次是一些函数不同平台下实现细节的差异

*   1.在ubuntu下获取Report格式的listctrl某一列的text 代码如下

            wxListItem info;
    	info.SetId(row);
    	info.SetColumn(col);
    	list-&gt;GetItem(info);

    而在xp中必需在list-&gt;GetItem(info) 之前设置item的text码：info.SetMask(wxLIST_MASK_TEXT);
*   2.wxDC类中设置放大系数和正负逻辑方向的一些不同，参见以前的有关讨论。
<!--more-->

### 最多的是一些界面实现的差异，最好用wxSizer类进行布局解决此问题。

*   1.绝对定位布局可能在不同系统下有很大差异
*   2.toolbar在xp中最好和其他控件一起进行sizer布局，毕竟toolbar也是控件，实际上它就是继承自wxControl类。
*   3.在xp下面默认字体有点小，可以在顶级窗口中用以下语句进行改变，子窗口默认继承父窗口的字体
SetFont(wxFont(11,wxFONTFAMILY_DEFAULT,wxFONTSTYLE_NORMAL,wxFONTWEIGHT_NORMAL) );
*   4.可以在visual C++中用资源管理器添加ICON，然后再顶级窗口中用下列语句添加图标，这样编译出来的可执行程序默认就有好看的图标了
SetIcon(wxIcon(wxT("IDI_ICON_MAIN")) );//IDI_ICON_MAIN为添加的ICON的ID
*   5.很多默认的行为不一样，比如在Ubuntu下为Dialog设置可放大边框后自然会有最大化框，但在xp下面必需设置wxMAXIMIZE_BOX样式，其他很多默认行为也不一样，所以最好清楚指明窗口和控件的样式