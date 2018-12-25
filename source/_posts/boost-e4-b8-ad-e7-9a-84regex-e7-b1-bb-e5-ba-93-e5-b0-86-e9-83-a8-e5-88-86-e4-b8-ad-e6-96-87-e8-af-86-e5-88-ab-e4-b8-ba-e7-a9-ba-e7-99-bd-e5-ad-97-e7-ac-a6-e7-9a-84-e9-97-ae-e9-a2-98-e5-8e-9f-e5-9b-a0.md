---
title: Boost中的Regex类库将部分中文识别为空白字符的问题原因及解决办法
tags:
  - C++
  - regex
  - 中文
  - 空白
id: 1173
categories:
  - C++
date: 2012-03-13 17:52:15
---

问题描述：
使用字符类\s匹配一个字符串中的空白字符时，部分中文字符也将被识别为空白。

原因：
查看Boost的Regex源代码可以发现，Regex使用cpp_regex_traits类(在文件 boost/regex/v4/cpp_regex_traits.hpp 中定义)来处理字符类

<pre lang='cpp'>
// class cpp_regex_traits_base:
// acts as a container for locale and the facets we are using.
//
template <class charT>
struct cpp_regex_traits_base
{
   cpp_regex_traits_base(const std::locale& l)
   { imbue(l); }
   std::locale imbue(const std::locale& l);

   std::locale m_locale;
   std::ctype<charT> const* m_pctype; //这个类用来识别空白符
//……
}
</pre>

可以看到Regex使用[std::ctype](http://www.cplusplus.com/reference/std/locale/ctype/)类来识别空白符等
ctype类有一个[is成员函数](http://www.cplusplus.com/reference/std/locale/ctype/is/)用来判断某个字符是否属于空白字符或数字字符等，regex正是使用了这个成员函数。
查看这个成员函数的介绍可知字符类是在[cctype](http://www.cplusplus.com/reference/clibrary/cctype/)头文件中定义的
cctype头文件定义了一系列函数来分类和转换单个字符，函数isspace来判断一个字符是否为空白字符
再来看函数[isspace](http://www.cplusplus.com/reference/clibrary/cctype/isspace/)的说明，可知在C++中,指定了locale的此函数的模板版本存在于头文件<locale>中.
也就是说指定不同的locale，此函数的行为将不同。而默认的locale为"C" locale集。这就是问题的根源。

解决办法：1.使用[ \t\r\n]等特定的字符来代替\s
2.设置合适的locale并使用宽字符集和Regex的宽字符版本wregex