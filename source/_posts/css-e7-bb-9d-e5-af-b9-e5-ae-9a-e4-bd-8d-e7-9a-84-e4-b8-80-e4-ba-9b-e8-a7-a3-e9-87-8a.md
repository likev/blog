---
title: CSS绝对定位的一些解释
tags:
  - css
  - 定位
  - 浮动
id: 1002
categories:
  - html
date: 2011-11-13 20:01:09
---

<pre lang='html4strict'>
<!doctype html>
<html>
<head>
<meta charset=uft-8>
<title> absolute定位实验</title>
<script src='https://ajax.googleapis.com/ajax/libs/jquery/1.7.0/jquery.min.js'></script>

<style>
#a, #b, .c, .d{
text-align:center;
}
#a{
position:absolute;
left:200px;
top:100px;
width:600px;
border:1px red solid;
}

#b{
position:absolute;
bottom:20px;
right:10px;
width:200px;
height:100px;
border:1px blue solid;
}
.c{
float:left;
width:200px;
height:100px;
border:1px blue solid;
}
.d{
float:left;
width:200px;
height:300px;
border:1px blue solid;
}
</style>

</head>

<body>
<div id=a>absoluteA<div id=b>absoluteB</div><div class=c>floatC</div><div class=d>floatD</div></div>
</body>
<head>

</pre>

效果如下：
[![css定位](http://grow-wordpress.stor.sinaapp.com/uploads/2011/11/position-300x165.png "点击查看大图")](http://grow-wordpress.stor.sinaapp.com/uploads/2011/11/position.png)

可以看到：

1.  采用absolute定位时，left,right,top,bottom分别是定位元素与父元素 左-左 右-右 上-上 下-下 边的距离
2.  float元素的父元素为非绝对定位元素时，float不会撑大父元素的高度。当float元素的父元素为绝对定位元素时，float元素会撑大父元素的宽度和高度
3.  当absolute定位的元素(比如元素M)内容改变时，定位属性不会改变。比如指定M的bottom为10px，当动态向M添加了一些内容导致M高度增大时，M将向上面伸展，底框与父元素始终保持10px