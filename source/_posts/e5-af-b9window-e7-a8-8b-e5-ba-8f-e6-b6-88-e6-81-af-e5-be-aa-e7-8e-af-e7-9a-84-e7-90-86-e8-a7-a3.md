---
title: 对Window程序消息循环的理解
tags:
  - window
  - 消息循环
id: 1193
categories:
  - C++
date: 2012-03-26 18:26:07
---

*   ### 1.每个(创建窗口的)线程有一个消息队列，程序用下面的循环接收、转换消息，并将消息分发到合适的窗口处理程序：

<pre lang="cpp">
    MSG msg = { };
    while (GetMessage(&msg, NULL, 0, 0))
    {
        TranslateMessage(&msg);
        DispatchMessage(&msg);
    }
</pre>
*   ### 2.windows系统负责把消息放入每个线程的消息队列或者直接调用合适的窗口处理程序

*   ### 3.[Post消息和Send消息的区别](http://msdn.microsoft.com/en-us/library/ff381405%28v=vs.85%29.aspx#posted_messages_versus_sent_messages)

> a. Post一个消息(可以调用API函数[PostMessage](http://msdn.microsoft.com/en-us/library/ms644944%28v=vs.85%29.aspx))表示消息将经过消息队列，通过消息循环来分发消息> 
> b. Send一个消息(可以调用API函数[Send<span style="font-family: Consolas;">Message</span>](http://msdn.microsoft.com/en-us/library/ms644950%28v=vs.85%29.aspx))表示消息会跳过消息队列，操作系统直接调用窗口处理程序
*   ### 4.可以在任意线程中发送自定义的消息(消息值&gt;= WM_USER)到指定的窗口

*   ### 5.[消息队列](http://msdn.microsoft.com/en-us/library/ms644927%28v=vs.85%29.aspx#quequed_messages)

操作系统维护一个系统消息队列并为每一个GUI线程维护一个线程消息队列。为了避免为非GUI线程创建消息队列的开销，所有的线程在最初创建时没有消息队列。仅当线程第一次调用特定的用户函数时系统才创建一个线程消息队列；没有任何GUI函数的调用会导致消息队列的创建。

*   ### 6.队列消息和非队列消息

a. 队列消息
> 移动或点击鼠标、敲击键盘等大部分消息为队列消息。> 
> 仅当消息队列中没有其它消息时，**WM_PAINT**、**WM_TIMER**、**WM_QUIT**消息才被发送到窗口处理程序。> 
> 其它的消息按先进先出的原则被发送到窗口处理程序> 
> 用户可以用PostMessage等函数来发送一个队列消息
b. 非队列消息
> 比如当窗口转为active状态时，或者用户调用某些系统函数(如**[SetWindowPos](http://msdn.microsoft.com/en-us/library/ms633545%28v=vs.85%29.aspx)**)时，消息将跳过消息队列，直接发往窗口处理程序。> 
> 用户可以调用SendMessage等函数来发送一个非队列消息