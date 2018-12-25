---
title: C++程序配置类库
tags:
  - C++
  - config
  - library
  - 类库
  - 配置
id: 1143
categories:
  - C++
date: 2012-03-07 10:28:12
---

### 一、INI文件读取库

除了使用Windows提供的API函数(见[之前文章](http://grow.sinaapp.com/?p=988)介绍)和[Boost](http://www.boost.org)、[QT](http://qt.nokia.com/products/)、[wxWidgets](http://www.wxwidgets.org/)等类库提供的配置函数外，还可以使用下面的类库：

#### 1.SimpleIni([code.jellycan.com/simpleini/](http://code.jellycan.com/simpleini/))

一个跨平台的类库，提供简单的API读写INI文件，支持ASCII, MBCS and Unicode文件格式。开源，使用MIT协议。
使用方法：
<pre lang="cpp">
	CSimpleIniA ini;
	ini.SetUnicode();
	ini.LoadFile("myfile.ini");
	const char * pVal = ini.GetValue("section", "key", "default");
	ini.SetValue("section", "key", "newvalue");
</pre>

#### 2.RudeConfig([rudeserver.com/config/index.html](http://rudeserver.com/config/index.html))

<pre lang="cpp">
	// Create config object
	//
	Config config;

	// load a configuration/.ini file
	//
	config.load("myfile.ini");

	// read information
	//
	config.setSection("General Info");
	double cost = config.getDoubleValue("Cost");
	const char *company = config.getStringValue("Company Name");

	// create information
	//
	config.setSection("new section");
	config.setStringValue("animal type", "giraffe");
	config.setBoolValue("mammal", true);

	// save changes
	//
	config.save();
</pre>

#### 3.minIni([code.google.com/p/minini/](http://code.google.com/p/minini/))

minIni是一个在嵌入式系统中使用的读取INI文件库。minIni占用极少资源，可以为各种文件IO库配置。

### 二、XML文件读取库

#### 1.TinyXML-2([grinninglizard.com/tinyxml2docs](http://www.grinninglizard.com/tinyxml2docs/index.html))

如名字所示，是简单的XML文件读取库，并且是第二版。仅包含一个.h文件和一个.cpp文件，直接和自己的源代码一起编译即可使用。

### 三、序列化文件(类似JSON格式)读取库

#### 1.libconfig([hyperrealm.com/libconfig/](http://www.hyperrealm.com/libconfig/))

Libconfig是一个简单的用来处理结构化配置文件的库，像这样的文件：[test.cfg](http://www.hyperrealm.com/libconfig/test.cfg.txt)。这种文件格式比XML更紧凑易读。不像XML，它是可识别类型的，所以在程序代码中不必做字符串解析。
<pre lang="cpp">
	int var1;
	double var2;
	const char *var3;

	if(config.lookupValue("values.var1", var1)
	 && config.lookupValue("values.var2", var2)
	 && config.lookupValue("values.var3", var3))
	{
	// use var1, var2, var3
	}
	else
	{
	// error handling here
	}
</pre>