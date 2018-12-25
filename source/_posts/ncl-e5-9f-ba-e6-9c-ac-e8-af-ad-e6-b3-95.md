---
title: NCL语言基本语法
tags:
  - ncl
  - 中文
  - 函数
  - 变量
  - 操作符
  - 表达式
  - 语句
  - 语法
  - 语言
id: 910
categories:
  - NCL
  - 编程
date: 2011-10-22 16:50:31
---

### 一、数据类型

1.[数值类型](http://www.ncl.ucar.edu/Document/Manuals/Ref_Manual/NclDataTypes.shtml#BasicNumericTypes)：
`integer、uint、short、ushort、byte、ubyte、long、ulong、double`
2.[非数值类型](http://www.ncl.ucar.edu/Document/Manuals/Ref_Manual/NclDataTypes.shtml#Non-numericTypes)：
`logical、string、character、graphic、file、list`

字符串(string)可以用双引号包围的一些字符生成（"This is an string"），和Javascript类似，字符串可以用加号(+)来连接。它本身不是数组，不可以用数组下标来获取子字符串，但是可以利用[一些函数](http://www.ncl.ucar.edu/Document/Functions/string.shtml)来操作和处理字符串。

### 二、变量

1.命名规则
和C语言一样，NCL语言中的变量名命名规则是：以字母或下划线开头的字母数字下划线组合。变量名区分大小写。

以下NCL关键字不可用于变量名：
`begin        break        byte        character        continue        create        defaultapp        do        double        else        end        enumeric        external	False        file        float        function        getvalues        graphic        group        if        integer        int64        list        load        local        logical        long        new        _Missing        Missing        new        noparent        numeric        procedure        quit        QUIT        Quit        record        return        setvalues        short        snumeric        stop
`
2.定义和使用变量
NCL中的变量定义规则和Javascript语言相似：无需声明即可使用，其类型由其值决定。和Javascript变量相似的另一面是变量可以拥有属性。
<pre lang='bash'>
a = (/27.2, -10.0/)
a@_FillValue = -10.0
b = a * 9.0/5.0 + 32.0
print(b)
</pre>
3.变量维度

NCL中的多维数组使用 行 x 列 的方式储存，这点和C语言一致。按照约定，维度值为0 到 n-1，这里 n 是数据的维度。维度数值是有意义的，因为NCL允许将名称和维度进行关联。这样方便了坐标系下标操作和名称下标操作。变量维度以下列方式命名：
`temperature!0 = "frtime"
    temperature!1 = "lat"
    temperature!2 = "lon"
`

4.坐标变量

坐标变量是一些一维向量，并且和它们被指定的维度拥有相同的名称和大小。这些向量代表了每一个命名维度的数据坐标。如果这些向量中的值是单调递增或者递减，它们可以在坐标系下标操作中被使用。坐标变量定义如下：
`temperature&frtime = forecast_times
    temperature&lat = lat_points
    temperature&lon = lon_points
`

### 三、操作符和表达式

1.操作符和优先级如下
a.数值运算操作符
<table>
<tr><td>() 括号</td></tr>
<tr><td>- 取负(注意其优先级较高，和其他编程语言不同)</td></tr>
<tr><td>^ 乘方 数字的乘方或者数组的乘方 结果恒为浮点型，除非操作数为双精度型</td></tr>
<tr><td>
		*	乘

		/	除

		%	取模 两边的操作数必须均为整数

		#	矩阵乘法

</td></tr>
<tr><td>
		+	加 数值相加，如果两边是字符串，则连接两个字符串

		-	减

</td></tr>
<tr><td>
		&lt;	小于选择符(注意不是逻辑上的小于) arrayA &lt; arrayB 的结果为一个数组arrayC，arrayC[i]为arrayA[i]和arrayB[i]中较小的一个

		&gt;	大于选择符(注意不是逻辑上的大于) arrayA &gt; arrayB 的结果为一个数组arrayC，arrayC[i]为arrayA[i]和arrayB[i]中较大的一个

</td></tr>
</table>

b.逻辑操作符
<pre>
		.le. 	小于等于(less-than-or-equal)
		.lt.	小于(less-than)
		.ge.	大于等于(greater-than-or-equal)
		.gt.	大于(greater-than)
		.ne.	不等于(not-equal)
		.eq.	等于(equal)
		.and.	且
		.xor.	亦或(exclusive-or)
		.or.	或
		.not.	非
</pre>

c.数组操作符

数组操作符可以组合一组标量值或其他数组为新的数组。一个数组操作符由逗号(,)分割并用'(/' 和 '/)' (称为数组设计符)包围。数组可以由任何基本类型或图形(graphical)对象组成，目前不支持文件数组。每一个被逗号分割的元素必须拥有相同的维度。如果元素类型不同，默认用[强制转换规则](http://www.ncl.ucar.edu/Document/Manuals/Ref_Manual/NclDataTypes.shtml#Coercion)将所有元素转换为相同的类型。

下面是一些数组操作符的例子：

    (/ 1, 2, 3, 4, 5 /)
    (/ (/ 1, 2, 3 /)^2, (/ 4, 5, 6 /)^3,(/ 7, 8, 9 /)^4 /)
    (/ a - b, b + c, c / d /)

d.数组下标操作
NCL中的数组下标操作和Fortran类似，除了下面几点不同：
i)NCL下标范围为[0,n-1] 
ii)NCL中对于坐标变量(coordinate variables)的下标操作是对坐标变量中的数据进行操作
iii)命名的下标使用维度的名字以允许对数组重排序

下标操作示例：
`temperature(0,5,6) 
temperature(1:3,5,6)
temperature(1:3,4:5,5:6)
temperature(0:4:2,0:5:3,0:6:4)
temperature(3:1,5,6)
temperature(3:1,4:5,5:6)
temperature(:2,:1,5:)
temperature(:,:,:)
temperature(:2:-1,:1:-1,5::-1)
temperature(::-1,::-1,::-1) 反转数组
temperature((/1,1,1,2,2,2,/),:,:) 使用向量作为第一个下标

坐标系下标操作
temperature(0,{20:60},{-95:-120})
temperature(0,{20},{-95})
temperature(0,{:20:2},{:-95:2})

名称下标操作
temperature( time | 0, lon | :, lat | : )
temperature( time | :, {lon | 20 : 60}, {lat | -95 : -120})
`

### 四、NCL 语句

1.块语句(Blocks)

块语句提供了一种将一系列命令分组的方式。
`
    begin
        statement list
    end
`
当以加载脚本(loading scripts)或管道脚本(piping scripts)方式使用NCL时必须使用块语句

2.if 语句
`
if(scalar_logical_expression) then
    statement list
end if

if( scalar_logical_expression) then
    statement list
else
    statement list
end if
`
3.do 循环语句
`
        statement list
    end do 

    do loop_identifier = scalar_start_expr , scalar_end_expr , scalar_stride_expr
        statement list
    end do 
`
4.while 循环语句
`
do while (scalar_logical_expression)
    statement list
end do 
`
5.赋值语句

'->'、 '!'、 '&' 和 '@' 构造符被用来指定文件变量声明、维度名称声明、坐标变量声明和属性声明。没有这些构造符时，将进行普通的值-变量 赋值。

6.函数语句

NCL中有两种可重用的代码片段：函数(Function)和过程(procedure)，这点和Fortran及Matlab语言类似。函数和过程有相似的定义语法，唯一的区别是function和procedure关键字。函数定义方法如下：
`
    function function_name ( declaration_list )
    local local_identifier_list
    begin
        statement list
        return(return_value) 
    end
`

### 五、NCL 输入输出(IO)

1\. 输入输出[支持格式](http://www.ncl.ucar.edu/Document/Manuals/Ref_Manual/NclFormatSupport.shtml)的文件
[addfile](http://www.ncl.ucar.edu/Document/Functions/Built-in/addfile.shtml)

2\. 输入输出ascii文件
[asciiread](http://www.ncl.ucar.edu/Document/Functions/Built-in/asciiread.shtml) [asciiwrite](http://www.ncl.ucar.edu/Document/Functions/Built-in/asciiwrite.shtml)

3.输入输出二维数组(矩阵)
[write_matrix](http://www.ncl.ucar.edu/Document/Functions/Built-in/write_matrix.shtml)