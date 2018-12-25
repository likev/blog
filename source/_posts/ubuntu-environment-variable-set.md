---
title: Ubuntu 环境变量的设置
tags:
  - 变量
  - 环境
  - 系统
  - 设置
id: 1051
categories:
  - ubuntu
date: 2011-12-12 09:58:13
---

# 持久性的环境变量

到目前为止，我们只讨论临时设置一个环境变量的方式，当设置它时所在的shell会话被关闭时这个环境变量也就失效了。有人可能会问，是否有一种方法来永久设置一个环境变量为特定的值。

**Note:** 下面提到的Shell配置文件只为特定Shells和桌面环境所读取，不应该被以其他方式使用。

<!-- more -->

## 1. 会话范围环境变量

只影响特定用户的环境变量 (而不是整个系统)应该在下面文件中设置:

*   **~/.pam_environment** - 这个文件是特别为设置用户的环境变量.它并不是一个脚本文件，而是由每行一句声明表达式组成

    **Note:** 使用 .pam_environment 需要重新登录以便初始化环境变量. 仅仅重新打开 terminal 并不能够立即使用这些变量.

    如果你正在使用 KDE, 请查看 [the KDE User-base page on this topic](http://userbase.kde.org/Session_Environment_Variables/en).

不推荐在下面文件中设置:

*   **~/.profile** - This is probably the best file for placing environment variable  assignments, since it gets executed automatically by the Display** **Manager during the start-up process desktop session as well as by the login shell when one logs-in from the textual console.

*   **~/.bash_profile** or **~./bash_login** - If one of these file exist, bash executes it rather then "~/.profile"  when it is started as a login shell. (Bash will prefer  "~/.bash_profile" to "~/.bash_login"). However, these files won't  influence a graphical session by default.

*   **~/.bashrc** - Because of the way Ubuntu currently sets up the various script files  by default, this may be the easiest place to set variables in. The  default configuration nearly guarantees that this file will be executed  in each and every invocation of bash as well as while logging in to the  graphical environment. However, performance-wise this may not be the  best thing to do since it will cause values to be unnecessarily set many  times.

## 2. 系统范围环境变量

影响整个系统的环境变量设置 (而不是仅仅一个用户) 不应该放在任何系统或桌面会话加载时被执行的系统级别的脚本中，而应该在下面文件中设置：

*   **/etc/environment** - 这个文件是特别为设置系统范围的环境变量. 它并不是一个脚本文件，而是由每行一句声明表达式组成. 特别地，这个文件存储了系统范围的 locale 和 path 设置.
不推荐在以下文件中设置:

*   **/etc/profile** - This file gets executed whenever a bash login shell is entered (e.g.  when logging in from the console or over ssh), as well as by the Display** **Manager  when the desktop session loads. This is probably the file you will get  referred to when asking veteran UNIX system administrators about  environment variables. In Ubuntu, however, this file does little more  then invoke the _/etc/bash.bashrc_ file.

*   **/etc/bash.bashrc** - This is the system-wide version of the _~/.bashrc_ file. Ubuntu is configured by default to execute this file whenever a user enters a shell or the desktop environment.

**Note:** 当处理多用户桌面系统时，把设置放在上面提到的用户的~/.pam_environment 文件中是比较合适的，而不是系统范围的文件，因为这些文件不需要root权限来编辑，并且很容易在多个系统中移动。


>原文链接：[https://help.ubuntu.com/community/EnvironmentVariables](https://help.ubuntu.com/community/EnvironmentVariables)
