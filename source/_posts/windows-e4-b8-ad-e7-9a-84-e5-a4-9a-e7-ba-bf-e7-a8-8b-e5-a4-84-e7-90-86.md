---
title: windows中的多线程处理
tags:
  - window
  - 创建
  - 多线程
  - 通讯
id: 1203
categories:
  - C++
date: 2012-03-26 18:34:08
---

### （一）建立新线程的函数

1.Win32 API函数 [CreateThread](http://msdn.microsoft.com/en-us/library/ms682453%28v=vs.85%29.aspx)
<pre lang='cpp'>HANDLE WINAPI CreateThread(
  __in_opt   LPSECURITY_ATTRIBUTES lpThreadAttributes,
  __in       SIZE_T dwStackSize,
  __in       LPTHREAD_START_ROUTINE lpStartAddress,
  __in_opt   LPVOID lpParameter,
  __in       DWORD dwCreationFlags,
  __out_opt  LPDWORD lpThreadId
);</pre>

2.也可以用C运行库的函数 [_beginthread](http://msdn.microsoft.com/en-us/library/kdzttdcb%28v=vs.80%29.aspx) 来创建新线程
<pre lang='cpp'>uintptr_t _beginthread( 
   void( *start_address )( void * ),
   unsigned stack_size,
   void *arglist 
);</pre>

### （二）线程间通讯方法：

1.消息通讯
可以在线程中用[SendMessage](http://msdn.microsoft.com/en-us/library/ms644950%28VS.85%29.aspx)发送自定义消息到指定窗口
<pre  lang='cpp'>LRESULT WINAPI SendMessage(
  __in  HWND hWnd,
  __in  UINT Msg,
  __in  WPARAM wParam,
  __in  LPARAM lParam
);</pre>

2.创建线程时可以传递一个结构体的指针
3.利用全局变量来通讯