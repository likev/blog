---
title: 在main之前运行代码
tags:
  - C++
  - main
  - 函数
id: 366
categories:
  - C++
date: 2010-12-30 14:01:25
---

我们学习C语言编程的时候老师都告诉我们程序从main函数开始执行，main返回时也代表程序结束。那么能否在main函数执行前运行一些代码呢，当然可以，虽然没多大意义。演示代码如下：
<pre lang="cpp">
#include <iostream>

class outNum{
public:
	outNum()
	{
		int a;
		std::cin>>a;
		std::cout<<a<<std::endl;
	}
};
int run()
{
	std::cout<<"runn";
	return 0;
}
int main()
{
	std::cout<<"beginn";
	return 0;
}
outNum a;
int m=run();
</pre>

上面代码运行后先执行outNum对象的创建，无参数构造函数要求输入一个整形值，比如我们输入22后运行结果如下：
<pre lang='cmd'>
22
22
run
begin
</pre>
记得以前哪本书上提到过在main运行前进行一些验证什么的。在这里用示例代码和大家分享一下。