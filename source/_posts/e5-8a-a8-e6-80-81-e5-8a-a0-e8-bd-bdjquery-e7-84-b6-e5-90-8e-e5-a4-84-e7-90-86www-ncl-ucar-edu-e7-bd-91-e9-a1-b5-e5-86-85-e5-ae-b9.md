---
title: 动态加载jQuery然后处理www.ncl.ucar.edu网页内容
id: 1062
categories:
  - 未分类
date: 2011-12-13 11:29:07
tags:
---

<pre lang='javascript'>
//----- 动态加载jQuery
var j = document.createElement('script');
j.src = 'https://ajax.googleapis.com/ajax/libs/jquery/1/jquery.min.js';

var h = document.getElementsByTagName('head')[0];

h.appendChild(j);

//------ 添加一个div用来保存结果
clear();
$('#wrap').prepend('<div id=result></div>');

//-------  处理resource名称
clear();
var dts = $('#general_main > dl >dt');
var titles='';
dts.each(function(){
var title = $(this).children('strong').text();
console.log(title);
titles += title + ',';
})

$('#result').text(titles);

//----- 处理默认值
clear();
var dts = $('#general_main > dl >dd');
var titles='';
dts.each(function(){
if($.trim($(this).text() )=='' ) return;

var title = $(this).find('p').last().text();
console.log(title);
if(title){
titles += title + '##';
}else{
titles +=  'novalue##';
}

})

$('#result').text(titles);
</pre>