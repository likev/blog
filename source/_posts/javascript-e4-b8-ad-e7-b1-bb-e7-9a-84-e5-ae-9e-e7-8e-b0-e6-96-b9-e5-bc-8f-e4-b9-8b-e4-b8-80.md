---
title: Javascript 中类的实现方式之一
id: 1215
categories:
  - javascript
date: 2012-04-09 11:49:23
tags:
---

世上本没有路，走的人多了……
Javascript中本没有类，但可以用函数来实现类。

先来看简单的矩形类Rect的实现：
<pre lang='javascript'>
function Rect(w,h){
    this.width = w;
    this.height = h;
}

var rect1 = new Rect(10,20);
window.alert('rect1.width = '+rect1.width);
</pre>
上面实现了Rect类，这个类有两个公开数据成员width和height。定义一个对象(或者叫类的一个实例)的方法是在函数前加上new关键字。
下面来看怎么定义私有数据成员：
<pre lang='javascript'>
function Rect(w,h){
    var width = w, height = h;

    this.getWidth = function(){
        return width;
    }
    this.getHeight = function(){
        return height;
    }
}

var rect1 = new Rect(10,20);
window.alert('rect1.width = '+rect1.getWidth());
</pre>
上面将width和height定义为私有数据成员，并定义了两个公开成员函数getWidth和getHeight。
可见，定义私有数据成员或者私有成员函数的方法实际上是将他们定义为函数内部变量。

另外需要特别说明的是：一般情况下，在函数Rect内部，私有成员函数只可以访问私有成员（私有数据成员或者私有成员函数），而公开成员函数可以访问所有成员，这一点和我们熟悉的面向对象方法不太一样。