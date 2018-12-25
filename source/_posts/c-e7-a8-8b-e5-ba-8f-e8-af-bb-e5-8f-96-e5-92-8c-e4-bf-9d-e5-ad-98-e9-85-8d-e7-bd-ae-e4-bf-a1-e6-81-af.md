---
title: C++程序读取和保存配置信息
tags:
  - C++
  - 代码
  - 函数
  - 读取
  - 配置
id: 988
categories:
  - C++
  - 编程
date: 2011-11-10 11:06:07
---

虽然MSDN推荐使用注册表代替ini文件来保存程序配置和运行信息，但一般的小程序还是用ini文件来保存信息比较方便一些。

微软提供了GetPrivateProfile和WritePrivateProfile开头的一组函数来读取和保存ini文件。
比如对于名称为scan.ini的配置文件
<pre lang='ini'>
[lastest]
year =2011
month =11
day =8
hour =19
minute =0
second =56
</pre>

读取时间信息的代码如下
<pre lang='cpp'>
CTime get_last_time()
{
	int year,month,day,hour,minute,second;

	year   = GetPrivateProfileInt("lastest","year",1970,"./scan.ini");
	month  = GetPrivateProfileInt("lastest","month",1,"./scan.ini");
	day    = GetPrivateProfileInt("lastest","day",2,"./scan.ini");
	hour   = GetPrivateProfileInt("lastest","hour",0,"./scan.ini");
	minute = GetPrivateProfileInt("lastest","minute",0,"./scan.ini");
	second = GetPrivateProfileInt("lastest","second",0,"./scan.ini");

	return CTime(year,month,day,hour,minute,second);
}
</pre>

写入时间信息的代码如下
<pre lang='cpp'>
bool set_latest_time(const CTime &latest)
{
	BOOL year,month,day,hour,minute,second;

	year   = WritePrivateProfileString("lastest","year",latest.Format("%Y"),"./scan.ini");
	month  = WritePrivateProfileString("lastest","month",latest.Format("%#m"),"./scan.ini");
	day    = WritePrivateProfileString("lastest","day",latest.Format("%#d"),"./scan.ini");
	hour   = WritePrivateProfileString("lastest","hour",latest.Format("%#H"),"./scan.ini");
	minute = WritePrivateProfileString("lastest","minute",latest.Format("%#M"),"./scan.ini");
	second = WritePrivateProfileString("lastest","second",latest.Format("%#S"),"./scan.ini");

	return year && month && day && hour && minute && second;
}
</pre>