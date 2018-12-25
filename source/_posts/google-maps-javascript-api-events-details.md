---
title: Google Maps JavaScript API 几种事件(event)的说明
tags:
  - Ajax
  - event
  - Google
  - maps
  - 事件
  - 顺序
id: 1041
categories:
  - html
  - javascript
date: 2011-11-29 19:07:39
---

当移动或放大缩小google maps时，将会产生zoom_changed、center_changed、bounds_changed、dragend等各种事件。通过下面的html代码可以测试这些事件何时发生，以及发生的先后顺序。

运行html文件后可得出下面的结论：

1.  当移动地图时，center_changed和bounds_changed事件会不断触发，一直到移动结束。所以如果需要在视图改变时利用Ajax方式获取数据时千万不要绑定到bounds_changed(或center_changed)事件，因为这样会在移动一次地图时触发多次bounds_changed事件，导致多次重复的Ajax请求
2.  事件触发的顺序 center_changed -- zoom_changed --  bounds_changed ， 当center_changed事件发生时不一定能正确通过getBounds()函数获取视图边界
3.  dragend事件在拖动结束时触发，此时由于地图可能还在移动，所以还可能继续触发center_changed和bounds_changed事件

<!-- more -->

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Google Maps JavaScript API v3 Example: Event Simple</title>
    <meta name="viewport" content="initial-scale=1.0, user-scalable=no">
    <meta charset="UTF-8">

	<style>
	html, body {
		height: 100%;
		margin: 0;
		padding: 0;
	}
	#map_canvas {
		height: 100%;
	}
	html, body {
		height: auto;
	}
	#map_canvas {
		height: 650px;
	}

</style>

<script src="https://ajax.googleapis.com/ajax/libs/jquery/1.7.0/jquery.min.js"></script>
    <script type="text/javascript"
        src="http://maps.googleapis.com/maps/api/js?sensor=false"></script>
    <script type="text/javascript">
      function initialize() {
        var myOptions = {
          zoom: 4,
          center: new google.maps.LatLng(35.363882, 125.044922),
          mapTypeId: google.maps.MapTypeId.ROADMAP
        };

        var map = new google.maps.Map(document.getElementById('map_canvas'),
            myOptions);

		function getinfo(type){
			var center = map.getCenter();
			$('#info').append('
'+type+'
 lat:'+center.lat() + '  lng:'+ center.lng());
		}

        google.maps.event.addListener(map, 'zoom_changed', function() {
			getinfo('zoom_changed');
        });
		google.maps.event.addListener(map, 'bounds_changed', function() {
			getinfo('bounds_changed');
        });
		google.maps.event.addListener(map, 'center_changed', function() {
			getinfo('center_changed');
        });
		google.maps.event.addListener(map, 'dragend', function() {
			getinfo('dragend');
        });
      }

      google.maps.event.addDomListener(window, 'load', initialize);
    </script>

  </head>
  <body>
  <div id="map_canvas"></div>
	<div id='info'></div>

  </body>
</html>

```
