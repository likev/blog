---
title: C++跨平台开源库POCO学习笔记
tags:
  - poco
  - 手册
  - 文档
  - 类库
id: 1271
categories:
  - C++
date: 2012-12-20 10:49:49
---

POCO([pocoproject.org](http://pocoproject.org/ "POCO官方网站"))看起来是很不错的C++跨平台开源库，包含网络(HTTP、FTP等)、正则、XML、Zip、日期、文件、线程、通知、配置、日志、Timer等方面的类，只可惜国内使用者和讨论很少。

### 一、编译安装方法

1.  从官网([pocoproject.org/download](http://pocoproject.org/download/index.html "点击进入官网下载"))下载POCO源代码，推荐下载基本版本(Basic Edition)
2.  POCO由基础(Foundation)、有用工具(Util)、网络(Net)、XML等几大模块组成，源代码中每个模块为一个单独的目录，包含本模块的include文件、源代码(src)、例子(samples)和测试样本(testsuite)。

3. windows平台下推荐通过VS命令工具进行编译，具体操作为从开始--打开VS命令工具--进入poco源代码目录--输入buildwin查看具体用法。可选择生成3种不同的库(static_mt|static_md|shared|all)，还可选择生成release或debug版本，推荐生成release的static_mt版本，这样生成的程序可以直接发布。具体说明可参加官方文档中的说明([pocoproject.org/docs](http://pocoproject.org/docs/ "打开POCO官方文档"))。

	也可直接进入poco-1.4.6p4\Foundation 等源代码目录，打开sln文件(visual C++解决方案文件)，然后编译生成库文件，效果和前者相同(其实前者也是调用相应的sln文件)

	生成的库文件在源代码目录下的lib文件夹中

4.  可将各个不同模块下的include目录放在一起方便随后程序使用，像我这样
[![](http://grow-wordpress.stor.sinaapp.com/uploads/2012/12/poco.jpg "poco include目录")](http://grow-wordpress.stor.sinaapp.com/uploads/2012/12/poco.jpg)


### 二、如何使用呢--以免费的Visual C++ 2010 Express版本为例

1.  首先新建一个项目，添加一个C++源文件，点击Visual C++菜单栏的项目-属性打开属性页，点击 配置属性-C/C++-常规 在右边的附件包含目录里填入Poco的include文件所在目录。点击 配置属性-链接器-常规 在右边的附加库目录里填入Poco lib库或dll库所在的目录

2.  默认情况下Poco可自动链接生成的dll库，<del>如果想让它自动链接静态lib库，请点击 配置属性-C/C++-预处理器 在右边的预处理器定义中添加 POCO_STATIC，</del>最新版也可直接链接静态库。进一步了解请参考官方文档。

3.  Poco使用了C++的命名空间和异常机制，请记得处理异常哦，否则程序可能会崩溃的。Poco::Exception是所有Poco异常类的基类，如果你不知道具体的异常类型，可使用下面的方式捕获所有异常信息：

```cpp
try
{
	std::vector<std::string> dirs;
	getDirList(dirs);

	for(size_t i=0; i<dirs.size(); i++)
	{
		std::cout<<"deal dir "<<dirs[i]<<"....\n";
		pocoFtp1(dirs[i]);
	}
}
catch(Poco::Exception &exc)
{
	std::cout<<"exc"<<exc.displayText();
}
```


### 三、利用POCO进行HTTP POST请求的例子

```cpp
#include<iostream>
#include "Poco/Net/HTMLForm.h"
#include "Poco/URI.h"
#include "Poco/Net/HTTPClientSession.h"
#include "Poco/Net/HTTPRequest.h"
#include "Poco/Net/HTTPResponse.h"
#include "Poco/StreamCopier.h"
#include "Poco/Net/NetException.h"

//可用下面数据测试
//url http://current.sinaapp.com/post.php
//key abc
//value 456

//向网页提交post请求
void pocoPost(const std::string &url, const std::string &key, const std::string &value)
{
	Poco::URI purl(url);

	try
	{
		Poco::Net::HTTPClientSession session( purl.getHost(), purl.getPort() );
//如需设置代理 将下面一句注释去掉		
//session.setProxy("172.18.172.251",80);

		Poco::Net::HTTPRequest req(Poco::Net::HTTPRequest::HTTP_POST, purl.getPath(), Poco::Net::HTTPMessage::HTTP_1_1);

		Poco::Net::HTMLForm form;
		form.add(key, value);

		// Send the request.
		form.prepareSubmit(req);
		std::ostream& ostr = session.sendRequest(req);
		form.write(ostr);//提交post的键值信息

		Poco::Net::HTTPResponse res;

		std::istream& istr = session.receiveResponse(res);
//上句接收网站回应的信息 返回输入流 并copy到标准控制台输出流
		Poco::StreamCopier::copyStream(istr, std::cout);
		std::cout<<std::endl;
	}
	catch(Poco::Net::NetException& ex)
	{
		std::cout<<"post wrong: "<<ex.displayText();
	}
}
```

### 四、利用POCO操作FTP的例子

```cpp
#include "Poco/Net/FTPClientSession.h"
#include "Poco/StreamCopier.h"

#include <iostream>
#include <vector>
#include <sstream>

void pocoFtp(const std::string &host,const std::string &username,const std::string &password,const std::string &dir)
{
	Poco::Net::FTPClientSession session(host);
	session.login(username, password);//登录

	session.setWorkingDirectory(dir);//设置读取目录
	std::istream &ftpin = session.beginList("");//下载目录中文件列表

	std::string str;
	std::vector<std::string > filelist;
	while(ftpin>>str)
	{//存储文件列表
		filelist.push_back(str);
	}
	session.endList();//关闭目录下载连接

	for(size_t i=0; i!=filelist.size(); i++)
	{
		std::cout<<"deal file "<<filelist[i]<<"...\n";
		std::string content;
//下载每个文件并存储到字符串content中
		Poco::StreamCopier::copyToString( session.beginDownload( filelist[i] ), content);
		session.endDownload();//关闭下载连接
	}

	session.close();//断开FTP
}
```

### 五、利用POCO读写XML配置文件的例子

```cpp
#include "Poco/Util/XMLConfiguration.h"
#include <string>
#include <iostream>

void pocoConfig()
{
	using Poco::AutoPtr;
	using Poco::Util::XMLConfiguration;

	AutoPtr<XMLConfiguration> pConf(new XMLConfiguration("config1.xml") );

	pConf->setDouble("prop6",3.14);
	double a = pConf->getDouble("prop2");
	std::cout<<a;
	pConf->save("config1.xml");
}
```

xml配置文件格式如下
```xml
<config>
	<prop2>2.3</prop2>
</config>
```


相关资源：
>1. <a href="http://sdrv.ms/10E2YNR" title="点击查看" target="_blank">POCO官方幻灯片教程整理</a>
>2. [POCO官方文档说明](http://pocoproject.org/docs/ "点击查看")
