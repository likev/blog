---
title: 使用wxWidgets时发现的一些bug及解决方案
tags:
  - bug
  - C++
  - wxGTK
  - wxWidgets
id: 263
categories:
  - C++
  - ubuntu
  - wxWidgets
date: 2010-10-14 03:40:01
---

Ubuntu中

wxDC类

bug 1.  使用SetLogicalOrigin时必须确保坐标轴为默认方向（SetAxisOrientation(true,false)）,使用后可更改为需要的方向(SetAxisOrientation(true,true));

解决方案：查看wxGTK源代码文件dc.cpp可看到如下代码：
<pre lang='cpp'>
void wxDC::SetLogicalOrigin( wxCoord x, wxCoord y )
{
	m_logicalOriginX = x * m_signX;   // is this still correct ?
	m_logicalOriginY = y * m_signY;
	ComputeScaleAndOrigin();
}
</pre>

作者也察觉到了这里可能有问题，标注了// is this still correct ?

将上面代码修改如下即可：

<pre lang='cpp'>
void wxDC::SetLogicalOrigin( wxCoord x, wxCoord y )
{
	m_logicalOriginX = x ;
	m_logicalOriginY = y ;
	ComputeScaleAndOrigin();
}
</pre>
bug 2\. 使用SetUserScale函数设置放大倍数时画笔（wxPen）的宽度随之放大，但在xp系统下画笔宽度不变。也就是说如果设置SetUserScale(1,1000),则画笔宽度可能变为1000像素，导致无法成功绘制图像。

解决方案：从源代码文件dc.cpp中我们可以看到SetUserScale函数的定义：
<pre lang='cpp'>
void wxDC::SetUserScale( double x, double y )
{
	// allow negative ? -> no
	m_userScaleX = x;
	m_userScaleY = y;
	ComputeScaleAndOrigin();
}
</pre>

在源代码文件dcclient.cpp中我们可以看到wxWindowDC::ComputeScaleAndOrigin()函数的定义：

<pre lang='cpp'>
void wxWindowDC::ComputeScaleAndOrigin()
{
	const wxRealPoint origScale(m_scaleX, m_scaleY);

	wxDC::ComputeScaleAndOrigin();

	// if scale has changed call SetPen to recalulate the line width
	if ( wxRealPoint(m_scaleX, m_scaleY) != origScale && m_pen.Ok() )
	{
		// this is a bit artificial, but we need to force wxDC to think the pen
		// has changed
		wxPen pen = m_pen;
		m_pen = wxNullPen;
		SetPen( pen );
	}
}
</pre>

进一步我们可以找到函数 wxWindowDC::SetPen 的定义

<pre lang='cpp'>
void wxWindowDC::SetPen( const wxPen &pen )

{

	wxCHECK_RET( Ok(), wxT(“invalid window dc”) );
	if (m_pen == pen) return;
	m_pen = pen;
	if (!m_pen.Ok()) return;
	if (!m_window) return;

	gint width = m_pen.GetWidth();
	if (width <= 0)
	{
		// CMB: if width is non-zero scale it with the dc
		width = 1;
	}
	else
	{
		// X doesn’t allow different width in x and y and so we take
		// the average
		double w = 0.5 +
			( fabs((double) XLOG2DEVREL(width)) +
			fabs((double) YLOG2DEVREL(width)) ) / 2.0;
		width = (int)w;   //注意，这个宽度是最终绘制的宽度
		if ( !width )
		{
			// width can’t be 0 or an internal GTK error occurs inside
			// gdk_gc_set_dashes() below
			width = 1;
		}
	}

	//…… 中间的代码省略

	gdk_gc_set_line_attributes( m_penGC, width, lineStyle, capStyle, joinStyle );

	m_pen.GetColour().CalcPixel( m_cmap );

	gdk_gc_set_foreground( m_penGC, m_pen.GetColour().GetColor() );

}
</pre>

综合以上代码分析我们可以看到：当我们调用函数SetUserScale 放大绘制的图形时，wxGTK同时放大了绘制线条的宽度。

解决办法是删除 width = (int)w;  这行代码。

修改源代码后，重新编译wxGTK即可。

XP中

wxDateTime

bug 1\. wxDateTime::Format 函数不支持中文字符的格式化。

解决方案：暂时可以使用wxString::Format函数替代。