---
title: wxWidgets中定时器(wxTimer)的使用
tags:
  - C++
  - wxTimer
  - wxWidgets
id: 308
categories:
  - C++
  - wxWidgets
date: 2010-12-15 06:47:28
---

## 最简单的例子：

<pre lang='cpp'>
class MyFrame : public wxFrame
{
public:
...
       void OnTimer(wxTimerEvent&amp;amp; event);

private:
       wxTimer m_timer; //定义 wxTimer对象
};

BEGIN_EVENT_TABLE(MyFrame, wxFrame)
     EVT_TIMER(TIMER_ID, MyFrame::OnTimer) //绑定事件处理函数
END_EVENT_TABLE()

MyFrame::MyFrame()
: m_timer(this, TIMER_ID) //绑定此对象到this并指定TIMER_ID
{
       m_timer.Start(1000);    // 设置1秒间隔，并启动它
}

void MyFrame::OnTimer(wxTimerEvent&amp;amp; event)
{
     // 在下面写需要执行的代码
}
</pre>
<!--more-->

## 3种具体使用的方法

*   1\. 从 wxTimer 继承一个新的类并重载  Notify 成员函数来指定需要执行的功能.
*   2\. 使用非默认的构造函数或者 SetOwner成员指定消息通知对象(必须继承自 wxEvtHandler对象)，然后使用 EVT_TIMER 宏将它连接到接收 wxTimerEvent 消息的处理函数.
*   3\. 你也可以使用继承类并使用宏 EVT_TIMER 将它链接到一个消息处理函数. 由于它本身也是继承自wxEvtHandler，在使用默认构造函数的情况下, 接收消息的对象将是它自身 .
在任何一种情况下，需要在构造后使用Start 方法启动它，使用Stop方法关闭它。

Note: Timer 只能在主线程中使用.