---
title: C++ 字符串字面值的使用
tags:
  - C++
  - 字符串
  - 字符数组
  - 字面值
id: 1182
categories:
  - C++
date: 2012-03-25 00:05:55
---

以下语句将输出helloworld
```cpp
//code1
	char *a = "helloworld";

	std::cout<<a<<std::endl;
```
上面的a实际上是指向字符串字面值常量的起始地址，如果对a指向的字符进行赋值将会出现错误(比如 *(a+1) = 'E' 将出错)。
实际上应该像下面这样定义指针a(上面那样定义也能编译通过，但不推荐):
```cpp
//code2
	const char *a = "helloworld";
```

也可以用字符串字面值初始化字符数组，这样可以将字符数组当成字符串来使用：
```cpp
//code3
	char b[] = "helloworld";

	std::cout<<b<<std::endl;
```
注意上面是用字符串字面值来初始化字符数组b，数组b的长度为11，最后一位b[10] = '\0'. 可以直接在cout语句中输出b所存储的字符串的值，和code1类似。
但是请注意b为字符数组，数组b中的字符是可以改变的
```cpp
//code4
	char b[] = "helloworld";

	b[0] = 'H';
	std::cout<<b<<std::endl;
```
上面代码将输出Helloworld,第一个字符由小写h修改为大写H。

稍微深入一点来说：
每个程序在内存中都有一块区域来存放常量、字符串字面值常量等。当用字符指针的方式来定义一个字符串时，实际上是将指针指向了字符串字面值常量的起始地址。
当用字符数组的方式来定义字符串时，程序首先开辟一段新的内存，然后将字符串字面值常量复制到这个位置。

可以用下面的程序来验证这点
```cpp
#include <iostream>

int main()
{
	const char* p1 = "helloworld";
	char array1[]  = "helloworld";
	const char* p2 = "helloworld";

	std::cout<<" p1's address: "<<int(p1)
		<<"\n array1's address:"<<int(array1)
		<<"\n p2's address: "<<int(p2)<<std::endl;

}
```

上面程序输出为：
```
 p1's address: 13072640
 array1's address:1899864
 p2's address: 13072640
```

可以看到p1和p2指向相同的地址，而array1则为新的地址