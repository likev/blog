---
title: jqPlot选项结构
tags:
  - jqplot
  - option
  - 结构
  - 绘图
  - 选项
id: 1026
categories:
  - javascript
date: 2011-11-25 18:11:08
---

jqPlot是一个非常易用和强大的jQuery绘图插件，可以绘制曲线图、饼状图、柱状图等，支持多达9个Y坐标轴，能自动生成趋势线，可自定义坐标系、坐标轴、线条类型颜色、标签方向、图例、高亮数据点、鼠标提示字符串格式等各个绘图细节。官方网站为[www.jqplot.com](http://www.jqplot.com) ,基本使用步骤见[http://www.jqplot.com/docs/files/usage-txt.html](http://www.jqplot.com/docs/files/usage-txt.html) 。

绘制图形的语句为 `chart = $.jqplot('chart', data, optionsObj);`

$.jqplot函数有三个参数，第一个为div的ID，第二个为数据，第三个为绘图选项。

<!-- more -->

选项对象的结构如下：
```
jqPlot-|
       |-seriesColors(Array)
       |-textColor
       |-fontFamily
       |-fontSize
       |-stackSeries
       |-series(Array)-|
       |               |-Series1-|
       |               |         |-lineWidth
       |               |         |-shadow
       |               |         |-showLine
       |               |         |-showMarker
       |               |         |-color
       |               |         |-renderer
       |               |         |-rendererOptions
       |               |         |-trendline
       |               |-Series2...
       |               |-...
       |               |-SeriesN
       |
       |-grid(Object)-|
       |              |-drawGridLines
       |              |-background
       |              |-borderColor
       |              |-borderWidth
       |              |-shadow
       |
       |-title(Object)-|
       |               |-text
       |               |-show
       |               |-fontFamily
       |               |-fontSize
       |               |-textAlign
       |               |-textColor
       |
       |-axes(Object)-|
       |              |-xais-|
       |              |      |-min
       |              |      |-max
       |              |      |-numberTicks
       |              |      |-showTicks
       |              |      |-showTickMarks
       |              |      |-pad
       |              |      |-ticks
       |              |      |-tickOptions
       |              |      |-renderer
       |              |      |-rendererOptions
       |
       |-legend-|
       |        |-show
       |        |-location
       |
       |-cursor
       |
       |-dragable
       |
       |-highlighter
       |	   
       | ... and so on
```
