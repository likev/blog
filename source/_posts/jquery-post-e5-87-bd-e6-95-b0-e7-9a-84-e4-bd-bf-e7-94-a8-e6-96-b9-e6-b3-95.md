---
title: jQuery.post()函数的使用方法
tags:
  - Ajax
  - jquery
  - json
  - post
  - success
  - 函数
  - 类型
id: 760
categories:
  - javascript
date: 2011-08-20 23:54:37
---

函数原型： jQuery.post( url, [data], [success(data, textStatus, jqXHR)], [dataType] )
参数说明：
url 请求发送的地址
data 随请求发送的一个[关联对象](http://api.jquery.com/Types/#Map)或者一个字符串
success(data, textStatus, jqXHR)   指定请求成功时执行的一个callback函数
dataType 预期从服务器接收的数据类型. 默认: 智能判断  (xml, json, script, or html).

返回值类型：[jqXHR](http://api.jquery.com/jQuery.ajax/#jqXHR)

此函数是下面函数的简写形式
<pre lang='javascript'>
$.ajax({
  type: 'POST',
  url: url,
  data: data,
  success: success,
  dataType: dataType
});
</pre>

使用示例：
<pre lang='javascript'>
$.post("test.php", { "func": "getNameAndTime" },
 function(data){
   console.log(data.name); // John
   console.log(data.time); //  2pm
 }, "json")
.success(function() { alert("second success"); })
.error(function() { alert("error"); })
.complete(function() { alert("complete"); });
</pre>

关于dataType参数的[详细说明](http://api.jquery.com/jQuery.ajax/)
期待从服务器返回的数据类型. 如果不指定, jQuery 将基于返回结果的MIME类型 (XML MIME 类型将产生 XML, in 1.4 JSON 将产生 一个 JavaScript 对象, in 1.4 script 将执行 script, and 其他将作为字符串返回)尝试推断它. 可用的类型 (和传递给 success callback 函数第一个参数最终的结果) 是:

    "xml":  返回一个可以通过jQuery解析的 XML 文档  .

    "html":  把 HTML 作为普通文本返回; included script tags are evaluated when inserted in the DOM.

    "script":  将返回值作为 JavaScript对待并以普通文本方式返回. Disables caching by appending a query string parameter, "_=[TIMESTAMP]", to the URL unless the cache option is set to true. Note: This will turn POSTs into GETs for remote-domain requests.

    "json":  将返回值作为 JSON 对待 并返回一个 JavaScript 对象. In jQuery 1.4  JSON 数据使用严格的方式解析; 任何格式异常的JSON 都被拒绝并抛出一个parse error. (更多关于正确的JSON格式请参考 json.org 网站.)

    "jsonp":  Loads in a JSON block using JSONP. Adds an extra "?callback=?" to the end of your URL to specify the callback. Disables caching by appending a query string parameter, "_=[TIMESTAMP]", to the URL unless the cache option is set to true.

    "text":  普通文本字符串.

    多个以空格分隔的值: 从 jQuery 1.5, jQuery 能够将从Content-Type头中得到的dataType转换为你需要的其他类型 .  例如，如果你想将一个文本返回值作为XML对待，使用 "text xml" 作为 dataType. You can also make a JSONP request, have it received as text, and interpreted by jQuery as XML: "jsonp text xml." Similarly, a shorthand string such as "jsonp xml" will first attempt to convert from jsonp to xml, and, failing that, convert from jsonp to text, and then from text to xml.