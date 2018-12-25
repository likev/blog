---
title: CPP中多重 else if语句的简化
tags:
  - C++
  - 转化
id: 219
categories:
  - C++
date: 2009-12-19 14:14:30
---

函数
<pre lang='cpp'>
int ifelse(int m)
{
	if(m<10)
		return 5;
	else if(m<20)
		return 15;
	else if(m<30)
		return 25;
	else if(m<40)
		return 35;
	else if(m<50)
		return 45;
	else
		return 55;
}
</pre>

可以写为如下更简洁的形式
<pre lang='cpp'>
int ifelse(int m)
{
	return m<10 ? 5
		:  m<20 ? 15
		:  m<30 ? 25
		:  m<40 ? 35
		:  m<50 ? 45
		:  55;
}
</pre> 