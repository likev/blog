---
title: libcurl和libbzip2 windows平台编译和使用笔记
id: 1311
categories:
  - 未分类
date: 2014-07-03 18:09:24
tags:
---

## 版本及平台

<pre>
win7 
visual C++ 2010 express(学习版) 
curl-7.37.0 
bzip2 1.0.6
</pre>

## libcurl 编译

<pre lang='ini'>
打开vc命令行工具 进入源代码目录下的winbuild目录 执行 nmake /f Makefile.vc mode=<static or dll> <options>

<options>可以是下述的一个或多个选项:
   VC=<6,7,8,9,10,11,12>        - VC versions
   WITH_DEVEL=<path>            - Paths for the development files (SSL, zlib, etc.)
                                  Defaults to sibbling directory deps: ../deps
                                  Libraries can be fetched at http://pecl2.php.net/downloads/php-windows-builds/
                                  Uncompress them into the deps folder.
   WITH_SSL=<dll or static>     - Enable OpenSSL support, DLL or static
   WITH_ZLIB=<dll or static>    - Enable zlib support, DLL or static
   WITH_SSH2=<dll or static>    - Enable libSSH2 support, DLL or static
   ENABLE_IDN=<yes or no>       - Enable use of Windows IDN APIs, defaults to yes
                                  Requires Windows Vista or later, or installation from:
                                  http://www.microsoft.com/downloads/details.aspx?FamilyID=AD6158D7-DDBA-416A-9109-07607425A815
   ENABLE_IPV6=<yes or no>      - Enable IPv6, defaults to yes
   ENABLE_SSPI=<yes or no>      - Enable SSPI support, defaults to yes
   ENABLE_SPNEGO=<yes or no>    - Enable Simple and Protected GSSAPI Negotiation Mechanism, defaults to yes
   ENABLE_WINSSL=<yes or no>    - Enable native Windows SSL support, defaults to yes
   GEN_PDB=<yes or no>          - Generate Program Database (debug symbols for release build)
   DEBUG=<yes or no>            - Debug builds
   MACHINE=<x86 or x64>         - Target architecture (default x64 on AMD64, x86 on others)
</pre>
如果想修改 Runtime library 选项，可打开文件MakefileBuild.vc 修改下述配置
<pre># Runtime library configuration
# !IF "$(RTLIBCFG)"=="static"
!IF "$(MODE)"=="static"
RTLIB = /MT
RTLIB_DEBUG = /MTd
!ELSE
RTLIB = /MD
RTLIB_DEBUG  = /MDd
!ENDIF</pre>

## libcurl 使用

当使用静态库时 在程序代码开始处添加下述定义
#define CURL_STATICLIB
#include "curl/curl.h"

## libbzip2 编译

打开vc命令行工具 进入源代码目录 执行 nmake -f makefile.msc
makefile.msc 文件包含编译选项 如 -DWIN32 -MD -Ox -D_FILE_OFFSET_BITS=64 -nologo 可根据需要修改

## libbzip2 使用

仅需包含 bzlib.h 和 libbz2.lib