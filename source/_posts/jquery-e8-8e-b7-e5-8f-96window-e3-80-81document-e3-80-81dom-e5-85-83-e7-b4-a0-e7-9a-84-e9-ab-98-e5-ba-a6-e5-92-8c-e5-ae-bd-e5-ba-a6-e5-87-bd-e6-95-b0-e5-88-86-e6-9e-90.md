---
title: jQuery获取window、document、dom元素的高度和宽度函数分析
tags:
  - document
  - documentElement
  - height
  - jquery
  - width
  - window
  - 宽度
  - 文档
  - 窗口
  - 高度
id: 624
categories:
  - html
  - javascript
date: 2011-05-06 22:35:28
---

以下为获取高度或宽度函数的jQuery源代码
<pre lang="javascript">
// 创建jQuery.height(size)  jQuery.width(size)
//调用each方法创建两个相似的函数
jQuery.each([ "Height", "Width" ], function( i, name ) {

	var type = name.toLowerCase();

	jQuery.fn[ type ] = function( size ) {

		var elem = this[0];
		if ( !elem ) {
			return size == null ? null : this;
		}

		if ( jQuery.isFunction( size ) ) {
			return this.each(function( i ) {
				var self = jQuery( this );
				self[ type ]( size.call( this, i, self[ type ]() ) );
			});
		}

		// 获取window对象的高度或宽度 ($(window).width() ) 实际上是当前可见区域的高度或宽度
		if ( jQuery.isWindow( elem ) ) {
			// Everyone else use document.documentElement or document.body depending on Quirks vs Standards mode
			// 3rd condition allows Nokia support, as it supports the docElem prop but not CSS1Compat
			// 以上英文的意思是依赖于Quirks 或 Standards 文档模式来使用 
			// document.documentElement (实际上就是<html/>元素) 或 document.body
			var docElemProp = elem.document.documentElement[ "client" + name ];
			return elem.document.compatMode === "CSS1Compat" && docElemProp ||
				elem.document.body[ "client" + name ] || docElemProp;

		// 获取整个文档对象(document)的宽度或高度
		} else if ( elem.nodeType === 9 ) {
			// Either scroll[Width/Height] or offset[Width/Height], whichever is greater
			return Math.max(
				elem.documentElement["client" + name],
				elem.body["scroll" + name], elem.documentElement["scroll" + name],
				elem.body["offset" + name], elem.documentElement["offset" + name]
			);

		// 获取DOM元素的高度或宽度
		} else if ( size === undefined ) {
			var orig = jQuery.css( elem, type ),
				ret = parseFloat( orig );

			return jQuery.isNaN( ret ) ? orig : ret;

		// 设置DOM元素的高度或宽度 (当没有单位时默认为像素值)
		} else {
			return this.css( type, typeof size === "string" ? size : size + "px" );
		}
	};

});
</pre>
jQuery(window).height()代表了当前可见区域的大小，而jQuery(document).height()则代表了整个文档的高度，可视具体情况使用
注意当浏览器窗口大小改变时(如最大化或拉大窗口后) jQuery(window).height() 随之改变，但是jQuery(document).height()是不变的。