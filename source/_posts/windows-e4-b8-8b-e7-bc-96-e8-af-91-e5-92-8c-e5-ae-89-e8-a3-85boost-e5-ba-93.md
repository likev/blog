---
title: Windows下编译和安装Boost库的指定模块
tags:
  - boost
  - regex
  - VC
  - 单独编译
  - 配置
id: 1155
categories:
  - C++
date: 2012-03-07 16:17:04
---

当然你可以使用[www.boostpro.com](http://www.boostpro.com/download/)提供的安装工具来安装，免去以下的步骤。但是那会安装许多不必要的文件，占用大量磁盘空间，有可能使你更迷惑。可参见[这篇文章](http://blog.csdn.net/akof1314/article/details/6292980)。

如果你想了解如何一步步编译安装Boost库，请接着往下读。

一、到官网([www.boost.org](http://www.boost.org))下载最新版Boost并解压到任意目录
先来看一下解压后的目录结构，以$BOOST_ROOT代表你Boost所在的目录
<pre>
**$BOOST_ROOT****\** ................._boost 根目录_
   **index.htm** ........._A copy of www.boost.org starts here_
   **boost****\** ........................._所有的Boost头文件_
   **libs****\** ............_各种库的测试用例，文档说明。可以在这个文件夹中查看各种库怎么使用_
     **index.html** ........_库文档从这里开始_
     **algorithm****\**
     **any****\**
     **array****\**
                     _…更多的库…_
   **status****\** ........................._Boost范围测试套件_
   **tools****\** ..........._一些有用工具, 比如 Boost.Build, quickbook, bcp_
   **more****\** .........................._政策等其它文档._
   **doc****\** ..............._所有Boost库文档的子集_
</pre>

二、编译需要的库
首先要说明的是大多数Boost库现在**已经可以使用**了，直接包含boost目录下相应的头文件即可，并不需要编译安装。

以下是必须编译安装的Boost库：

*   [Boost.Filesystem](http://www.boost.org/doc/libs/1_49_0/libs/filesystem/index.html)
*   [Boost.GraphParallel](http://www.boost.org/doc/libs/1_49_0/libs/graph_parallel/index.html)
*   [Boost.IOStreams](http://www.boost.org/doc/libs/1_49_0/libs/iostreams/index.html)
*   [Boost.MPI](http://www.boost.org/doc/libs/1_49_0/libs/mpi/index.html)
*   [Boost.ProgramOptions](http://www.boost.org/doc/libs/1_49_0/libs/program_options/index.html)
*   [Boost.Python](http://www.boost.org/doc/libs/1_49_0/libs/python/doc/building.html) (see the [Boost.Python build documentation](http://www.boost.org/doc/libs/1_49_0/libs/python/doc/building.html)
before building and installing it)
*   [Boost.Regex](http://www.boost.org/doc/libs/1_49_0/libs/regex/index.html)
*   [Boost.Serialization](http://www.boost.org/doc/libs/1_49_0/libs/serialization/index.html)
*   [Boost.Signals](http://www.boost.org/doc/libs/1_49_0/libs/signals/index.html)
*   [Boost.System](http://www.boost.org/doc/libs/1_49_0/libs/system/index.html)
*   [Boost.Thread](http://www.boost.org/doc/libs/1_49_0/doc/html/thread.html)
*   [Boost.Wave](http://www.boost.org/doc/libs/1_49_0/libs/wave/index.html)

以下库拥有可选的编译组件(也就是说如果你要使用它们中的某些功能，则需要单独编译安装)

*   [Boost.DateTime](http://www.boost.org/doc/libs/1_49_0/libs/date_time/index.html) 当你使用它的 <tt class="docutils literal">to_string</tt>/<tt class="docutils literal">from_string</tt> 或者序列化特性, 或者目标平台为 Visual C++ 6.x 或 Borland.
*   [Boost.Graph](http://www.boost.org/doc/libs/1_49_0/libs/graph/index.html) 仅仅当你想 [处理 GraphViz 文件](http://www.boost.org/doc/libs/1_49_0/libs/graph/doc/read_graphviz.html).
*   [Boost.Math](http://www.boost.org/doc/libs/1_49_0/libs/math/index.html) 含有TR1 和 C99 cmath 函数二进制组件.
*   [Boost.Random](http://www.boost.org/doc/libs/1_49_0/libs/random/index.html) 当你使用 <tt class="docutils literal">random_device</tt>.
*   [Boost.Test](http://www.boost.org/doc/libs/1_49_0/libs/test/index.html) 可以 “header-only” 或 “separately compiled”
模式使用, 尽管 **对于郑重使用时推荐单独编译**.

如果要编译上面的库，首先打开命令行，转到$BOOST_ROOT目录并运行目录下的bootstrap.bat脚本，这个脚本为Boost.Build系统的运行准备环境。
<pre lang='cmd'>
bootstrap.bat
</pre>
可以看到现在$BOOST_ROOT目录下有b2.exe和bjam.exe两个可执行文件。这两个文件是一样的，只是名字不同，它们可以调用Boost.Build系统来创建上面那些需要编译安装的库。

比如我们想单独编译安装regex库，运行下面的命令即可
<pre lang='cmd'>
bjam stage --with-regex link=static threading=multi runtime-link=static
</pre>
下面介绍相关参数的含义：
stage 仅创建和安装库文件(不创建头文件),可以用 --stagedir=<STAGEDIR> 选项指定库的安装位置，默认安装在当前目录下的stage文件夹内。
  --with-<library> 创建和安装指定的库，如果使用了这个选项，则仅仅指定的库被创建，其它库不被创建。如果不指定这个选项，默认创建所有需要编译安装的库。
link=static指定生成静态regex库
threading=multi指定生成多线程库
runtime-link=static指定链接静态C和C++ 运行库

其他选项可参见[这篇文章](http://www.cnblogs.com/wondering/archive/2009/05/21/boost_setup.html)

三、配置开发环境
打开Visual Studio，在 工具->选项->项目和解决方案->VC++目录 条目下配置Boost包含文件和库文件目录，这样以后就不用每次都要配置Boost目录。