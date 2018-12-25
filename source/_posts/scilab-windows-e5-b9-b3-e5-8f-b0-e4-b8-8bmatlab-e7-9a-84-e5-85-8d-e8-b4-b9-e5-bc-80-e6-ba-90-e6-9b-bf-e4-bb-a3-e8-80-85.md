---
title: Scilab-Windows平台下MATLAB的免费开源替代者
tags:
  - MATLAB
  - Scilab
id: 1269
categories:
  - matlab
date: 2012-12-20 09:03:08
---

MATLAB很多人都听说过吧，大名鼎鼎售价昂贵的数值计算、可视化和编程开发软件，相信极少人用的是正版。推荐一款和MATLAB语法几乎100%兼容功能同样强大的免费开源软件Scilab，官方网站为[http://www.scilab.org/ ](http://www.scilab.org/ "http://www.scilab.org/") 同时欢迎与我交流。

将Scilab的函数列表([help.scilab.org/docs/5.4.0/en_US/index.html](http://help.scilab.org/docs/5.4.0/en_US/index.html "scilab 函数列表 官网"))翻译了一下，希望对大家有所帮助。

<a id="scilab_help_manual" name="scilab_help_manual" shape="rect" target="_blank"></a>
<div></div>

*   [Scilab](http://help.scilab.org/docs/5.4.0/ja_JP/section_c4c83f547edb45f8820db294bc05d947.html)

    *   配置[Configuration](http://help.scilab.org/docs/5.4.0/ja_JP/section_5ab2b7f6227403f45c04dd608af3979c.html)

            *   [banner](http://help.scilab.org/docs/5.4.0/ja_JP/banner.html) — 显示 Scilab 横幅
        *   [getdebuginfo](http://help.scilab.org/docs/5.4.0/ja_JP/getdebuginfo.html) — 获取 Scilab 的调试信息
        *   [getmemory](http://help.scilab.org/docs/5.4.0/ja_JP/getmemory.html) — 返回可用的系统内存和系统内存的总量
        *   [getmodules](http://help.scilab.org/docs/5.4.0/ja_JP/getmodules.html) — 返回安装在 Scilab 中的模块的列表
        *   [getos](http://help.scilab.org/docs/5.4.0/ja_JP/getos.html) — 返回操作系统版本的名称
        *   [getscilabmode](http://help.scilab.org/docs/5.4.0/ja_JP/getscilabmode.html) — Scilab 的设置模式
        *   [getshell](http://help.scilab.org/docs/5.4.0/ja_JP/getshell.html) — 返回当前命令解释程序。
        *   [getversion](http://help.scilab.org/docs/5.4.0/ja_JP/getversion.html) — 获取 Scilab 和模块的版本信息
        *   [gstacksize](http://help.scilab.org/docs/5.4.0/ja_JP/gstacksize.html) — 设置/获取全球的堆栈大小
        *   [stacksize](http://help.scilab.org/docs/5.4.0/ja_JP/stacksize.html) — 设置 scilab 的堆栈的大小
        *   [ver](http://help.scilab.org/docs/5.4.0/ja_JP/ver.html) — Scilab 的版本信息
        *   [with_javasci](http://help.scilab.org/docs/5.4.0/ja_JP/with_javasci.html) — 找出是否有 Scilab 包括一个 Java 接口
        *   [with_macros_source](http://help.scilab.org/docs/5.4.0/ja_JP/with_macros_source.html) — 要确定安装了宏的来源
        *   [with_module](http://help.scilab.org/docs/5.4.0/ja_JP/with_module.html) — 找出是否安装了 Scilab 模块
        *   [with_texmacs](http://help.scilab.org/docs/5.4.0/ja_JP/with_texmacs.html) — 找出是否由 texmacs 调用 Scilab
        *   [with_tk](http://help.scilab.org/docs/5.4.0/ja_JP/with_tk.html) — 检查是否在 Scilab 中安装了 Tcl/Tk

        *   控制流[Control flow](http://help.scilab.org/docs/5.4.0/ja_JP/control_flow.html)

            *   [abort](http://help.scilab.org/docs/5.4.0/ja_JP/abort.html) — 打出来。
        *   [break](http://help.scilab.org/docs/5.4.0/ja_JP/break.html) — 描述循环中断的关键字
        *   [case](http://help.scilab.org/docs/5.4.0/ja_JP/case.html) — 在选择使用关键字
        *   [continue](http://help.scilab.org/docs/5.4.0/ja_JP/continue.html) — 将控制转移到下一个循环迭代关键字
        *   [do](http://help.scilab.org/docs/5.4.0/ja_JP/do.html) — 语言关键字的 for 循环
        *   [for](http://help.scilab.org/docs/5.4.0/ja_JP/for.html) — 语言关键字的 for 循环
        *   [if](http://help.scilab.org/docs/5.4.0/ja_JP/if.html) — 有条件执行
        *   [pause](http://help.scilab.org/docs/5.4.0/ja_JP/pause.html) — 等待中断模式下，键盘输入
        *   [resume](http://help.scilab.org/docs/5.4.0/ja_JP/resume.html) — 当地人返回或恢复执行和副本
        *   [return](http://help.scilab.org/docs/5.4.0/ja_JP/return.html) — 返回或恢复，复制本地变量
        *   [select](http://help.scilab.org/docs/5.4.0/ja_JP/select.html) — 选择关键字
        *   [then](http://help.scilab.org/docs/5.4.0/ja_JP/then.html) — 如果那时其他关键字
        *   [while](http://help.scilab.org/docs/5.4.0/ja_JP/while.html) — 同时关键字

        *   调试[Debugging](http://help.scilab.org/docs/5.4.0/ja_JP/section_5c95314d1914b4c4234a3a8021689768.html)

            *   [debug](http://help.scilab.org/docs/5.4.0/ja_JP/debug.html) — 调试级别
        *   [delbpt](http://help.scilab.org/docs/5.4.0/ja_JP/delbpt.html) — 若要删除断点
        *   [dispbpt](http://help.scilab.org/docs/5.4.0/ja_JP/dispbpt.html) — 显示断点
        *   [setbpt](http://help.scilab.org/docs/5.4.0/ja_JP/setbpt.html) — 设置断点
        *   [where](http://help.scilab.org/docs/5.4.0/ja_JP/where.html) — 获取当前指令调用树
        *   [whereami](http://help.scilab.org/docs/5.4.0/ja_JP/whereami.html) — 查看当前订单宫廷

        *   错误处理[Error handling](http://help.scilab.org/docs/5.4.0/ja_JP/error_handling.html)

            *   [errcatch](http://help.scilab.org/docs/5.4.0/ja_JP/errcatch.html) — 捕获错误与 edebug
        *   [errclear](http://help.scilab.org/docs/5.4.0/ja_JP/errclear.html) — 清除错误
        *   [error](http://help.scilab.org/docs/5.4.0/ja_JP/error.html) — 错误消息
        *   [error_table](http://help.scilab.org/docs/5.4.0/ja_JP/error_table.html) — 错误消息表
        *   [iserror](http://help.scilab.org/docs/5.4.0/ja_JP/iserror.html) — 错误检查
        *   [lasterror](http://help.scilab.org/docs/5.4.0/ja_JP/lasterror.html) — 获取最近记录的错误消息
        *   [warning](http://help.scilab.org/docs/5.4.0/ja_JP/warning.html) — 警告消息

        *   关键字[Scilab keywords](http://help.scilab.org/docs/5.4.0/ja_JP/section_e0fe496f951dd8e815ea57c9da4b78a5.html)

            *   [ans](http://help.scilab.org/docs/5.4.0/ja_JP/ans.html) — 答案
        *   [backslash](http://help.scilab.org/docs/5.4.0/ja_JP/backslash.html) — 矩阵 (&amp;gt;) 左司。
        *   [brackets](http://help.scilab.org/docs/5.4.0/ja_JP/brackets.html) — ([，]) 从左和右圆括号
        *   [colon](http://help.scilab.org/docs/5.4.0/ja_JP/colon.html) — (:) 冒号运算符
        *   [comma](http://help.scilab.org/docs/5.4.0/ja_JP/comma.html) — (，) 列、 指令、 参数分隔符
        *   [comments](http://help.scilab.org/docs/5.4.0/ja_JP/comments.html) — 评论
        *   [comparison](http://help.scilab.org/docs/5.4.0/ja_JP/comparison.html) — 比较，关系运算符
        *   [dollar](http://help.scilab.org/docs/5.4.0/ja_JP/dollar.html) — ($)，最后的索引
        *   [dot](http://help.scilab.org/docs/5.4.0/ja_JP/dot.html) — (.) 符号
        *   [else](http://help.scilab.org/docs/5.4.0/ja_JP/else.html) — 如果那时其他关键字
        *   [elseif](http://help.scilab.org/docs/5.4.0/ja_JP/elseif.html) — 如果那时其他关键字
        *   [empty](http://help.scilab.org/docs/5.4.0/ja_JP/empty.html) — ([]) 空矩阵
        *   [end](http://help.scilab.org/docs/5.4.0/ja_JP/end.html) — end 关键字
        *   [equal](http://help.scilab.org/docs/5.4.0/ja_JP/equal.html) — (=) 比较，平等
        *   [extraction](http://help.scilab.org/docs/5.4.0/ja_JP/extraction.html) — 发展的矩阵和列表中的条目
        *   [global](http://help.scilab.org/docs/5.4.0/ja_JP/global.html) — 定义全局变量
        *   [hat](http://help.scilab.org/docs/5.4.0/ja_JP/hat.html) — (^) 电源
        *   [insertion](http://help.scilab.org/docs/5.4.0/ja_JP/insertion.html) — 部分转让给一个变量
        *   [left](http://help.scilab.org/docs/5.4.0/ja_JP/left.html) — [左的括号
        *   [less](http://help.scilab.org/docs/5.4.0/ja_JP/less.html) — (&amp;gt;) 大于比较
        *   [minus](http://help.scilab.org/docs/5.4.0/ja_JP/minus.html) — 变化，减法运算符 (-) 迹象
        *   [not](http://help.scilab.org/docs/5.4.0/ja_JP/not.html) — (~) 逻辑非
        *   [parents](http://help.scilab.org/docs/5.4.0/ja_JP/parents.html) — () 左和右圆括号
        *   [percent](http://help.scilab.org/docs/5.4.0/ja_JP/percent.html) — (%) 特殊字符
        *   [plus](http://help.scilab.org/docs/5.4.0/ja_JP/plus.html) — 加法运算符)
        *   [power](http://help.scilab.org/docs/5.4.0/ja_JP/power.html) — 幂运算符 (^，.^)
        *   [quote](http://help.scilab.org/docs/5.4.0/ja_JP/quote.html) — (') 转置运算符、 字符串分隔符
        *   [semicolon](http://help.scilab.org/docs/5.4.0/ja_JP/semicolon.html) — 末尾的表达和行分隔符
        *   [slash](http://help.scilab.org/docs/5.4.0/ja_JP/slash.html) — (/) 右司和反馈
        *   [star](http://help.scilab.org/docs/5.4.0/ja_JP/star.html) — 乘法运算符 password(*)
        *   [symbols](http://help.scilab.org/docs/5.4.0/ja_JP/symbols.html) — scilab 运算符名称
        *   [tilda](http://help.scilab.org/docs/5.4.0/ja_JP/tilda.html) — (~) 逻辑非
        *   [try](http://help.scilab.org/docs/5.4.0/ja_JP/try.html) — 开始在 catch 块的 try catch 控制指令

        *   变量[Variables](http://help.scilab.org/docs/5.4.0/ja_JP/section_fcce9d9e6e137bedba941c420ce373db.html)

            *   [Predefined variables](http://help.scilab.org/docs/5.4.0/ja_JP/section_612847520f2d75912f51d189c33e7414.html)

                    *   [SCI](http://help.scilab.org/docs/5.4.0/ja_JP/SCI.html) — 与 Scilab 变量的根路径。
            *   [SCIHOME](http://help.scilab.org/docs/5.4.0/ja_JP/SCIHOME.html) — 与 Scilab 会话历史记录文件和配置文件的路径。
            *   [TMPDIR](http://help.scilab.org/docs/5.4.0/ja_JP/TMPDIR.html) — 临时目录的路径
            *   [percenteps](http://help.scilab.org/docs/5.4.0/ja_JP/percenteps.html) — Epsilon （浮点相对精度）
            *   [percenti](http://help.scilab.org/docs/5.4.0/ja_JP/percenti.html) — 虚数单位
            *   [percentinf](http://help.scilab.org/docs/5.4.0/ja_JP/percentinf.html) — 英飞尼迪
            *   [percentnan](http://help.scilab.org/docs/5.4.0/ja_JP/percentnan.html) — 数字不
            *   [percentpi](http://help.scilab.org/docs/5.4.0/ja_JP/percentpi.html) — 一个直径圆的周长的比率

                *   [clear](http://help.scilab.org/docs/5.4.0/ja_JP/clear.html) — 清除变量
        *   [clearglobal](http://help.scilab.org/docs/5.4.0/ja_JP/clearglobal.html) — 删除全局变量
        *   [exists](http://help.scilab.org/docs/5.4.0/ja_JP/exists.html) — 若要检查变量
        *   [getvariablesonstack](http://help.scilab.org/docs/5.4.0/ja_JP/getvariablesonstack.html) — Scilab 变量名的堆栈上获取
        *   [isdef](http://help.scilab.org/docs/5.4.0/ja_JP/isdef.html) — 验证存在该变量
        *   [isglobal](http://help.scilab.org/docs/5.4.0/ja_JP/isglobal.html) — 检查该变量是否全球
        *   [names](http://help.scilab.org/docs/5.4.0/ja_JP/names.html) — scilab 名称语法
        *   [predef](http://help.scilab.org/docs/5.4.0/ja_JP/predef.html) — 变量的保护
        *   [who](http://help.scilab.org/docs/5.4.0/ja_JP/who.html) — 变量的列表
        *   [who_user](http://help.scilab.org/docs/5.4.0/ja_JP/who_user.html) — 获取用户定义的变量的列表
        *   [whos](http://help.scilab.org/docs/5.4.0/ja_JP/whos.html) — 获取长格式的变量的列表

        *   [exit](http://help.scilab.org/docs/5.4.0/ja_JP/exit.html) — 要退出当前 Scilab 会话
    *   [perl](http://help.scilab.org/docs/5.4.0/ja_JP/perl.html) — 为相应的操作系统调用 Perl 脚本文件
    *   [quit](http://help.scilab.org/docs/5.4.0/ja_JP/quit.html) — 减少的 Scilab 级别暂停或结束
    *   [scilab](http://help.scilab.org/docs/5.4.0/ja_JP/scilab.html) — R 频率执行 Scilab 和相关的工具的主要的 Unix 脚本
    *   [sethomedirectory](http://help.scilab.org/docs/5.4.0/ja_JP/sethomedirectory.html) — 设置 Scilab 主目录
    *   [startup](http://help.scilab.org/docs/5.4.0/ja_JP/startup.html) — 启动文件
    *   [testmatrix](http://help.scilab.org/docs/5.4.0/ja_JP/testmatrix.html) — 创建救生员，弗兰克这类特殊矩阵
    *   [with_gtk](http://help.scilab.org/docs/5.4.0/ja_JP/with_gtk.html) — 要确定是否用"GIMP 工具包"库生成 Scilab

*   **微积分[Differential Equations, Integration](http://help.scilab.org/docs/5.4.0/ja_JP/section_c15779f3f67b69a9d25b7ddb69783748.html)**

    *   [bvode](http://help.scilab.org/docs/5.4.0/ja_JP/bvode.html) — bvode 的一个简单的呼叫
    *   [dae](http://help.scilab.org/docs/5.4.0/ja_JP/dae.html) — 微分代数方程求解
    *   [daeoptions](http://help.scilab.org/docs/5.4.0/ja_JP/daeoptions.html) — 规划求解 dae 的 set 的选项
    *   [dasrt](http://help.scilab.org/docs/5.4.0/ja_JP/dasrt.html) — 零交叉 DAE
    *   [dassl](http://help.scilab.org/docs/5.4.0/ja_JP/dassl.html) — 微分代数方程
    *   [diff](http://help.scilab.org/docs/5.4.0/ja_JP/diff.html) — 离散微分和差分
    *   [feval](http://help.scilab.org/docs/5.4.0/ja_JP/feval.html) — 要计算的函数 （或外部例程）
    *   [impl](http://help.scilab.org/docs/5.4.0/ja_JP/impl.html) — 微分代数方程
    *   [int2d](http://help.scilab.org/docs/5.4.0/ja_JP/int2d.html) — 定义由正交和三个维正交的 2 维积分
    *   [int3d](http://help.scilab.org/docs/5.4.0/ja_JP/int3d.html) — 定义由正交和三个维正交 3D 积分
    *   [intc](http://help.scilab.org/docs/5.4.0/ja_JP/intc.html) — 柯西积分
    *   [integrate](http://help.scilab.org/docs/5.4.0/ja_JP/integrate.html) — 由求积公式的积分
    *   [intg](http://help.scilab.org/docs/5.4.0/ja_JP/intg.html) — 定积分
    *   [intl](http://help.scilab.org/docs/5.4.0/ja_JP/intl.html) — 柯西积分
    *   [intsplin](http://help.scilab.org/docs/5.4.0/ja_JP/intsplin.html) — 样条内插法的实验数据的集成
    *   [inttrap](http://help.scilab.org/docs/5.4.0/ja_JP/inttrap.html) — 由梯形规则的实验数据的集成
    *   [numdiff](http://help.scilab.org/docs/5.4.0/ja_JP/numdiff.html) — 数值的梯度估计
    *   [ode](http://help.scilab.org/docs/5.4.0/ja_JP/ode.html) — 常微分方程求解
    *   [ode_discrete](http://help.scilab.org/docs/5.4.0/ja_JP/ode_discrete.html) — 离散时间模拟常微分方程，规划求解
    *   [ode_optional_output](http://help.scilab.org/docs/5.4.0/ja_JP/ode_optional_output.html) — ode 求解器可选输出说明
    *   [ode_root](http://help.scilab.org/docs/5.4.0/ja_JP/ode_root.html) — 求解常微分方程规划求解的解决方案
    *   [odedc](http://help.scilab.org/docs/5.4.0/ja_JP/odedc.html) — 离散 ／ 连续颂规划求解
    *   [odeoptions](http://help.scilab.org/docs/5.4.0/ja_JP/odeoptions.html) — 要设置的选项的颂歌规划求解

*   **基本函数[Elementary Functions](http://help.scilab.org/docs/5.4.0/ja_JP/section_9b956636f846b2b06bbb127a2ad4daab.html)**

    *   [bitwise](http://help.scilab.org/docs/5.4.0/ja_JP/section_6bb166fa82a744d9f0c4eb49cdc28d1d.html)

            *   [bitand](http://help.scilab.org/docs/5.4.0/ja_JP/bitand.html) — 按位逻辑与 (AND)
        *   [bitcmp](http://help.scilab.org/docs/5.4.0/ja_JP/bitcmp.html) — 位的补充
        *   [bitget](http://help.scilab.org/docs/5.4.0/ja_JP/bitget.html) — 在指定的位置有点入门
        *   [bitor](http://help.scilab.org/docs/5.4.0/ja_JP/bitor.html) — 按位逻辑 (OR)
        *   [bitset](http://help.scilab.org/docs/5.4.0/ja_JP/bitset.html) — 在指定位置设置的位
        *   [bitxor](http://help.scilab.org/docs/5.4.0/ja_JP/bitxor.html) — 按位异或 (XOR)
        *   [isequalbitwise](http://help.scilab.org/docs/5.4.0/ja_JP/isequalbitwise.html) — 变量比较

        *   [Complex](http://help.scilab.org/docs/5.4.0/ja_JP/section_c70de6912ab5267e3107bfb4d448c289.html)

            *   [complex](http://help.scilab.org/docs/5.4.0/ja_JP/complex.html) — 若要计算复杂的数字。
        *   [conj](http://help.scilab.org/docs/5.4.0/ja_JP/conj.html) — 共轭
        *   [imag](http://help.scilab.org/docs/5.4.0/ja_JP/imag.html) — 虚数部分
        *   [imult](http://help.scilab.org/docs/5.4.0/ja_JP/imult.html) — 乘以虚构单位我
        *   [isreal](http://help.scilab.org/docs/5.4.0/ja_JP/isreal.html) — C 变量确定是否真实的或复杂的条目
        *   [real](http://help.scilab.org/docs/5.4.0/ja_JP/real.html) — 实数部分

        *   [Discrete mathematics](http://help.scilab.org/docs/5.4.0/ja_JP/section_263fb9f422c8bea558b009204f0ee3d4.html)

            *   [binomial](http://help.scilab.org/docs/5.4.0/ja_JP/binomial.html) — (2) 的概率分布
        *   [factor](http://help.scilab.org/docs/5.4.0/ja_JP/factor.html) — 保理业务几分钟解决方案功能
        *   [factorial](http://help.scilab.org/docs/5.4.0/ja_JP/factorial.html) — 阶乘的函数
        *   [gcd](http://help.scilab.org/docs/5.4.0/ja_JP/gcd.html) — 计算最大公约数
        *   [lcm](http://help.scilab.org/docs/5.4.0/ja_JP/lcm.html) — 最小公倍数
        *   [perms](http://help.scilab.org/docs/5.4.0/ja_JP/perms.html) — 向量组件的所有排列
        *   [primes](http://help.scilab.org/docs/5.4.0/ja_JP/primes.html) — 主要功能
        *   [rat](http://help.scilab.org/docs/5.4.0/ja_JP/rat.html) — 有理逼近的浮点数

        *   [elementarymatrices](http://help.scilab.org/docs/5.4.0/ja_JP/section_3e7661fd871e59f37ae5342d05a58b28.html)

            *   [diag](http://help.scilab.org/docs/5.4.0/ja_JP/diag.html) — 扩大或建造三对角矩阵
        *   [eye](http://help.scilab.org/docs/5.4.0/ja_JP/eye.html) — 恒等矩阵
        *   [ind2sub](http://help.scilab.org/docs/5.4.0/ja_JP/ind2sub.html) — 成下标字符与矩阵的线性索引的字符
        *   [linspace](http://help.scilab.org/docs/5.4.0/ja_JP/linspace.html) — 向量线性安排
        *   [logspace](http://help.scilab.org/docs/5.4.0/ja_JP/logspace.html) — 向量的对数的时间间隔
        *   [meshgrid](http://help.scilab.org/docs/5.4.0/ja_JP/meshgrid.html) — 创建一个 3 维数组或矩阵
        *   [ndgrid](http://help.scilab.org/docs/5.4.0/ja_JP/ndgrid.html) — 网格数组多维功能评价
        *   [ones](http://help.scilab.org/docs/5.4.0/ja_JP/ones.html) — 1 矩阵
        *   [rand](http://help.scilab.org/docs/5.4.0/ja_JP/rand.html) — 随机数的生成
        *   [squarewave](http://help.scilab.org/docs/5.4.0/ja_JP/squarewave.html) — 期间 2 ＊ 生成 %pi 方波
        *   [sub2ind](http://help.scilab.org/docs/5.4.0/ja_JP/sub2ind.html) — 要转换的线性索引矩阵下标字符
        *   [toeplitz](http://help.scilab.org/docs/5.4.0/ja_JP/toeplitz.html) — Toeplitz 矩阵
        *   [zeros](http://help.scilab.org/docs/5.4.0/ja_JP/zeros.html) — 零矩阵

        *   [Exponential](http://help.scilab.org/docs/5.4.0/ja_JP/section_59d22412394f82dec3668a734764dc83.html)

            *   [exp](http://help.scilab.org/docs/5.4.0/ja_JP/exp.html) — 指数的序列中的元素
        *   [expm](http://help.scilab.org/docs/5.4.0/ja_JP/expm.html) — 广场矩阵指数
        *   [log](http://help.scilab.org/docs/5.4.0/ja_JP/log.html) — 自然对数
        *   [log10](http://help.scilab.org/docs/5.4.0/ja_JP/log10.html) — 对数
        *   [log1p](http://help.scilab.org/docs/5.4.0/ja_JP/log1p.html) — 要严格计算自然对数的参数加一
        *   [log2](http://help.scilab.org/docs/5.4.0/ja_JP/log2.html) — 基地 2 对数
        *   [logm](http://help.scilab.org/docs/5.4.0/ja_JP/logm.html) — 方阵对数
        *   [polar](http://help.scilab.org/docs/5.4.0/ja_JP/polar.html) — 極座標形表达式
        *   [sqrt](http://help.scilab.org/docs/5.4.0/ja_JP/sqrt.html) — 平方根
        *   [sqrtm](http://help.scilab.org/docs/5.4.0/ja_JP/sqrtm.html) — 矩阵的平方根

        *   [Floating point](http://help.scilab.org/docs/5.4.0/ja_JP/section_05ee369f5fac712b94a775563f8d7335.html)

            *   [ceil](http://help.scilab.org/docs/5.4.0/ja_JP/ceil.html) — 总结
        *   [clean](http://help.scilab.org/docs/5.4.0/ja_JP/clean.html) — 明确矩阵 （小条目，舍入为零）
        *   [double](http://help.scilab.org/docs/5.4.0/ja_JP/double.html) — 将整数转换为双精度表示形式
        *   [fix](http://help.scilab.org/docs/5.4.0/ja_JP/fix.html) — 朝 0 舍入
        *   [floor](http://help.scilab.org/docs/5.4.0/ja_JP/floor.html) — 向下取整
        *   [format](http://help.scilab.org/docs/5.4.0/ja_JP/format.html) — 格式化和打印任何数目
        *   [frexp](http://help.scilab.org/docs/5.4.0/ja_JP/frexp.html) — 要拆卸的尾数和指数的浮点数，2 为基础。
        *   [ieee](http://help.scilab.org/docs/5.4.0/ja_JP/ieee.html) — 设置浮动点异常模式
        *   [int](http://help.scilab.org/docs/5.4.0/ja_JP/int.html) — 整数部分
        *   [isinf](http://help.scilab.org/docs/5.4.0/ja_JP/isinf.html) — 看到无尽的条目
        *   [isnan](http://help.scilab.org/docs/5.4.0/ja_JP/isnan.html) — 为"非数字"找到项
        *   [nearfloat](http://help.scilab.org/docs/5.4.0/ja_JP/nearfloat.html) — 检索的上一页或下一页的浮点数
        *   [nextpow2](http://help.scilab.org/docs/5.4.0/ja_JP/nextpow2.html) — 下列值中的 2 的幂的
        *   [number_properties](http://help.scilab.org/docs/5.4.0/ja_JP/number_properties.html) — 若要定义浮动小数点数字参数
        *   [round](http://help.scilab.org/docs/5.4.0/ja_JP/round.html) — 舍入政策

        *   [Integer representation](http://help.scilab.org/docs/5.4.0/ja_JP/section_3ddc131a7680ac0dd5b52ec03cbd6a10.html)

            *   [base2dec](http://help.scilab.org/docs/5.4.0/ja_JP/base2dec.html) — 将转换为一个整数，从 b 和基底的表达式
        *   [bin2dec](http://help.scilab.org/docs/5.4.0/ja_JP/bin2dec.html) — 将转换为二进制整数的表示形式
        *   [dec2base](http://help.scilab.org/docs/5.4.0/ja_JP/dec2base.html) — 将 10 个十进制 （字符串） 基 N 数字转换
        *   [dec2bin](http://help.scilab.org/docs/5.4.0/ja_JP/dec2bin.html) — 二进制表示形式
        *   [dec2hex](http://help.scilab.org/docs/5.4.0/ja_JP/dec2hex.html) — 16 十六进制表示的整数
        *   [dec2oct](http://help.scilab.org/docs/5.4.0/ja_JP/dec2oct.html) — 8 十进制表示的整数
        *   [hex2dec](http://help.scilab.org/docs/5.4.0/ja_JP/hex2dec.html) — 停用 16 十六进制表示的整数转换
        *   [oct2dec](http://help.scilab.org/docs/5.4.0/ja_JP/oct2dec.html) — 要转换 8 十六进制整数

        *   [matrixmanipulation](http://help.scilab.org/docs/5.4.0/ja_JP/section_2211b1552d432cda761da1d783fa09c3.html)

            *   [flipdim](http://help.scilab.org/docs/5.4.0/ja_JP/flipdim.html) — 反向沿指定维度的 x 的元素
        *   [matrix](http://help.scilab.org/docs/5.4.0/ja_JP/matrix.html) — 塑造成大不同的向量或矩阵矩阵
        *   [permute](http://help.scilab.org/docs/5.4.0/ja_JP/permute.html) — 更改数组的维数的顺序
        *   [pertrans](http://help.scilab.org/docs/5.4.0/ja_JP/pertrans.html) — 过度移位 (pertranspose)
        *   [repmat](http://help.scilab.org/docs/5.4.0/ja_JP/repmat.html) — 放置复制的数组 / 瓷砖
        *   [resize_matrix](http://help.scilab.org/docs/5.4.0/ja_JP/resize_matrix.html) — 创建一个新的矩阵，不同大小的
        *   [squeeze](http://help.scilab.org/docs/5.4.0/ja_JP/squeeze.html) — 挤压播放

        *   [matrixoperations](http://help.scilab.org/docs/5.4.0/ja_JP/section_21ff803e38cc39dcd6210cbc9f6950e2.html)

            *   [abs](http://help.scilab.org/docs/5.4.0/ja_JP/abs.html) — 绝对价值震级
        *   [cumprod](http://help.scilab.org/docs/5.4.0/ja_JP/cumprod.html) — 累积产品
        *   [cumsum](http://help.scilab.org/docs/5.4.0/ja_JP/cumsum.html) — 累积总和
        *   [kron](http://help.scilab.org/docs/5.4.0/ja_JP/kron.html) — 克罗内克产品 （......＊.top)
        *   [max](http://help.scilab.org/docs/5.4.0/ja_JP/max.html) — 最大值
        *   [min](http://help.scilab.org/docs/5.4.0/ja_JP/min.html) — 最小值
        *   [norm](http://help.scilab.org/docs/5.4.0/ja_JP/norm.html) — 矩阵范数
        *   [prod](http://help.scilab.org/docs/5.4.0/ja_JP/prod.html) — 产品
        *   [signm](http://help.scilab.org/docs/5.4.0/ja_JP/signm.html) — 矩阵 sign 函数
        *   [sum](http://help.scilab.org/docs/5.4.0/ja_JP/sum.html) — 总计 （列总） 总和的向量 / 矩阵的条目
        *   [tril](http://help.scilab.org/docs/5.4.0/ja_JP/tril.html) — 下三角矩阵
        *   [triu](http://help.scilab.org/docs/5.4.0/ja_JP/triu.html) — 左上三角

        *   [searchandsort](http://help.scilab.org/docs/5.4.0/ja_JP/section_806c84bcf833acca8a410dc9bf65db58.html)

            *   [dsearch](http://help.scilab.org/docs/5.4.0/ja_JP/dsearch.html) — 二进制搜索算法
        *   [gsort](http://help.scilab.org/docs/5.4.0/ja_JP/gsort.html) — 快速排序算法排序
        *   [lex_sort](http://help.scilab.org/docs/5.4.0/ja_JP/lex_sort.html) — 字典排序的矩阵的行
        *   [vectorfind](http://help.scilab.org/docs/5.4.0/ja_JP/vectorfind.html) — 找到一行或一列的矩阵的匹配矢量

        *   [setoperations](http://help.scilab.org/docs/5.4.0/ja_JP/section_fa3e34b1ea4f9833cadcae5c7b94b565.html)

            *   [intersect](http://help.scilab.org/docs/5.4.0/ja_JP/intersect.html) — 返回两个向量中的共同价值观的载体
        *   [setdiff](http://help.scilab.org/docs/5.4.0/ja_JP/setdiff.html) — 返回的不属于另一个向量的组件的一个向量的元素
        *   [union](http://help.scilab.org/docs/5.4.0/ja_JP/union.html) — 展开组件的矢量的总和
        *   [unique](http://help.scilab.org/docs/5.4.0/ja_JP/unique.html) — 向量或矩阵的唯一的元素

        *   [signalprocessing](http://help.scilab.org/docs/5.4.0/ja_JP/section_57d7e04ff1956cfba0511899fa2d1b54.html)

            *   [bloc2exp](http://help.scilab.org/docs/5.4.0/ja_JP/bloc2exp.html) — 块关系图符号的评价
        *   [bloc2ss](http://help.scilab.org/docs/5.4.0/ja_JP/bloc2ss.html) — 转型 b 座状态空间表示法
        *   [pen2ea](http://help.scilab.org/docs/5.4.0/ja_JP/pen2ea.html) — E、 A 转换从铅笔
        *   [ssrand](http://help.scilab.org/docs/5.4.0/ja_JP/ssrand.html) — 随机数生成器
        *   [sysconv](http://help.scilab.org/docs/5.4.0/ja_JP/sysconv.html) — 系统转换
        *   [sysdiag](http://help.scilab.org/docs/5.4.0/ja_JP/sysdiag.html) — 块对角系统连接
        *   [syslin](http://help.scilab.org/docs/5.4.0/ja_JP/syslin.html) — 若要定义一个线性系统
        *   [trfmod](http://help.scilab.org/docs/5.4.0/ja_JP/trfmod.html) — 杆 / 显示零

        *   [symbolic](http://help.scilab.org/docs/5.4.0/ja_JP/section_ee13c830839f1d7bf3109018d49c85da.html)

            *   [addf](http://help.scilab.org/docs/5.4.0/ja_JP/addf.html) — 象征性的加法
        *   [cmb_lin](http://help.scilab.org/docs/5.4.0/ja_JP/cmb_lin.html) — 一个象征性的线性组合
        *   [ldivf](http://help.scilab.org/docs/5.4.0/ja_JP/ldivf.html) — 象征性的左的司
        *   [mulf](http://help.scilab.org/docs/5.4.0/ja_JP/mulf.html) — 符号乘法
        *   [rdivf](http://help.scilab.org/docs/5.4.0/ja_JP/rdivf.html) — 象征性的右司
        *   [solve](http://help.scilab.org/docs/5.4.0/ja_JP/solve.html) — 代数线性系统求解器
        *   [subf](http://help.scilab.org/docs/5.4.0/ja_JP/subf.html) — 象征性的减法
        *   [trianfml](http://help.scilab.org/docs/5.4.0/ja_JP/trianfml.html) — 象征性的求解
        *   [trisolve](http://help.scilab.org/docs/5.4.0/ja_JP/trisolve.html) — 象征性的线性 システムソルバ

        *   [Trigonometry](http://help.scilab.org/docs/5.4.0/ja_JP/section_785e14288da064e9dce1291c9ce0f461.html)

            *   [acos](http://help.scilab.org/docs/5.4.0/ja_JP/acos.html) — 每个元素的反余弦值
        *   [acosd](http://help.scilab.org/docs/5.4.0/ja_JP/acosd.html) — 每个元素的反余弦值是结果。
        *   [acosh](http://help.scilab.org/docs/5.4.0/ja_JP/acosh.html) — 反双曲余弦值
        *   [acoshm](http://help.scilab.org/docs/5.4.0/ja_JP/acoshm.html) — 矩阵反双曲余弦值
        *   [acosm](http://help.scilab.org/docs/5.4.0/ja_JP/acosm.html) — 每个矩阵的反余弦值
        *   [acot](http://help.scilab.org/docs/5.4.0/ja_JP/acot.html) — 若要计算的参数序列中的元素的反正切。
        *   [acotd](http://help.scilab.org/docs/5.4.0/ja_JP/acotd.html) — 参数序列中的元素的逆正切值 （单位： 度） 来计算。
        *   [acoth](http://help.scilab.org/docs/5.4.0/ja_JP/acoth.html) — 反双曲正切值序列中的元素。
        *   [acsc](http://help.scilab.org/docs/5.4.0/ja_JP/acsc.html) — 若要计算参数的反余割函数的每个元素。
        *   [acscd](http://help.scilab.org/docs/5.4.0/ja_JP/acscd.html) — 计算的参数一次中返回的结果序列中的元素的反余割。
        *   [acsch](http://help.scilab.org/docs/5.4.0/ja_JP/acsch.html) — 若要计算参数的反双曲余割函数的每个元素。
        *   [asec](http://help.scilab.org/docs/5.4.0/ja_JP/asec.html) — 计算的参数序列中的元素的反正割。
        *   [asecd](http://help.scilab.org/docs/5.4.0/ja_JP/asecd.html) — 计算结果倍中的返回每个元素的参数，反正的割。
        *   [asech](http://help.scilab.org/docs/5.4.0/ja_JP/asech.html) — 计算的参数序列中的元素的反双曲正割。
        *   [asin](http://help.scilab.org/docs/5.4.0/ja_JP/asin.html) — 反正弦值
        *   [asind](http://help.scilab.org/docs/5.4.0/ja_JP/asind.html) — 反正弦值 (结果的单位： 次）
        *   [asinh](http://help.scilab.org/docs/5.4.0/ja_JP/asinh.html) — 反双曲正弦值
        *   [asinhm](http://help.scilab.org/docs/5.4.0/ja_JP/asinhm.html) — 矩阵双曲反正弦值
        *   [asinm](http://help.scilab.org/docs/5.4.0/ja_JP/asinm.html) — 为矩阵反正弦值
        *   [atan](http://help.scilab.org/docs/5.4.0/ja_JP/atan.html) — 2 象限和四象限的反正切
        *   [atand](http://help.scilab.org/docs/5.4.0/ja_JP/atand.html) — 2 象限和四象限反正，造成，以度为单位。
        *   [atanh](http://help.scilab.org/docs/5.4.0/ja_JP/atanh.html) — 反双曲正切值
        *   [atanhm](http://help.scilab.org/docs/5.4.0/ja_JP/atanhm.html) — 矩阵反双曲正切值
        *   [atanm](http://help.scilab.org/docs/5.4.0/ja_JP/atanm.html) — 方阵逆正切
        *   [cos](http://help.scilab.org/docs/5.4.0/ja_JP/cos.html) — 余弦函数
        *   [cosd](http://help.scilab.org/docs/5.4.0/ja_JP/cosd.html) — 每个元素的余弦值 （参数单位： 次)
        *   [cosh](http://help.scilab.org/docs/5.4.0/ja_JP/cosh.html) — 双曲余弦值
        *   [coshm](http://help.scilab.org/docs/5.4.0/ja_JP/coshm.html) — 矩阵双曲余弦值
        *   [cosm](http://help.scilab.org/docs/5.4.0/ja_JP/cosm.html) — 矩阵余弦函数
        *   [cotd](http://help.scilab.org/docs/5.4.0/ja_JP/cotd.html) — 余切 (股余切的参数： 倍）
        *   [cotg](http://help.scilab.org/docs/5.4.0/ja_JP/cotg.html) — 余切 (余切)
        *   [coth](http://help.scilab.org/docs/5.4.0/ja_JP/coth.html) — 双曲余切 (余切)
        *   [cothm](http://help.scilab.org/docs/5.4.0/ja_JP/cothm.html) — 矩阵双曲余切 (余切)
        *   [csc](http://help.scilab.org/docs/5.4.0/ja_JP/csc.html) — 若要计算参数 (余割） 序列中的元素的余割。
        *   [cscd](http://help.scilab.org/docs/5.4.0/ja_JP/cscd.html) — 时间来计算 (余割) 余割由序列中的元素指定的参数
        *   [csch](http://help.scilab.org/docs/5.4.0/ja_JP/csch.html) — 若要计算参数的双曲余割函数的每个元素。
        *   [csgn](http://help.scilab.org/docs/5.4.0/ja_JP/csgn.html) — 返回无符号的复杂向量的真实部分。
        *   [sec](http://help.scilab.org/docs/5.4.0/ja_JP/sec.html) — 若要计算参数的割线的每个元素。
        *   [secd](http://help.scilab.org/docs/5.4.0/ja_JP/secd.html) — 割线序列中的元素 （参数单位： 次）
        *   [sech](http://help.scilab.org/docs/5.4.0/ja_JP/sech.html) — 计算每个元素的参数的双曲正割
        *   [sin](http://help.scilab.org/docs/5.4.0/ja_JP/sin.html) — 正弦函数
        *   [sinc](http://help.scilab.org/docs/5.4.0/ja_JP/sinc.html) — Sinc 函数
        *   [sind](http://help.scilab.org/docs/5.4.0/ja_JP/sind.html) — 序列中的元素的正弦值 （参数单位： 度)。
        *   [sinh](http://help.scilab.org/docs/5.4.0/ja_JP/sinh.html) — 双曲正弦值
        *   [sinhm](http://help.scilab.org/docs/5.4.0/ja_JP/sinhm.html) — 矩阵双曲正弦值
        *   [sinm](http://help.scilab.org/docs/5.4.0/ja_JP/sinm.html) — 矩阵正弦函数
        *   [tan](http://help.scilab.org/docs/5.4.0/ja_JP/tan.html) — 切线
        *   [tand](http://help.scilab.org/docs/5.4.0/ja_JP/tand.html) — 耗散系数 （单位： 度）
        *   [tanh](http://help.scilab.org/docs/5.4.0/ja_JP/tanh.html) — 双曲正切值
        *   [tanhm](http://help.scilab.org/docs/5.4.0/ja_JP/tanhm.html) — 矩阵双曲正切值
        *   [tanm](http://help.scilab.org/docs/5.4.0/ja_JP/tanm.html) — 矩阵切线

        *   [and](http://help.scilab.org/docs/5.4.0/ja_JP/and.html) — 逻辑元素的数组
    *   [and_op](http://help.scilab.org/docs/5.4.0/ja_JP/and_op.html) — 逻辑运算符和运算符
    *   [cat](http://help.scilab.org/docs/5.4.0/ja_JP/cat.html) — 若要合并两个或多个数组
    *   [cell2mat](http://help.scilab.org/docs/5.4.0/ja_JP/cell2mat.html) — 单元格数组到一个矩阵
    *   [cellstr](http://help.scilab.org/docs/5.4.0/ja_JP/cellstr.html) — 转换字符串向量 （或字符串矩阵） 的单元格
    *   [isempty](http://help.scilab.org/docs/5.4.0/ja_JP/isempty.html) — 确定变量是否为空白或空的行和列列表
    *   [isequal](http://help.scilab.org/docs/5.4.0/ja_JP/isequal.html) — 比较对象
    *   [isvector](http://help.scilab.org/docs/5.4.0/ja_JP/isvector.html) — 确定如果变量向量
    *   [lstsize](http://help.scilab.org/docs/5.4.0/ja_JP/lstsize.html) — 列表、 tlist、 mlist 条目数
    *   [maxi](http://help.scilab.org/docs/5.4.0/ja_JP/maxi.html) — 最大值
    *   [mini](http://help.scilab.org/docs/5.4.0/ja_JP/mini.html) — 最小值
    *   [modulo](http://help.scilab.org/docs/5.4.0/ja_JP/modulo.html) — 求模和模 m 积极
    *   [ndims](http://help.scilab.org/docs/5.4.0/ja_JP/ndims.html) — 数组中的维度数
    *   [nthroot](http://help.scilab.org/docs/5.4.0/ja_JP/nthroot.html) — 第 n 个实数的真正根源
    *   [or](http://help.scilab.org/docs/5.4.0/ja_JP/or.html) — 对数组的元素的逻辑析取
    *   [or_op](http://help.scilab.org/docs/5.4.0/ja_JP/or_op.html) — 逻辑或运算符
    *   [sign](http://help.scilab.org/docs/5.4.0/ja_JP/sign.html) — Sign 函数
    *   [size](http://help.scilab.org/docs/5.4.0/ja_JP/size.html) — 对象的大小
    *   [sort](http://help.scilab.org/docs/5.4.0/ja_JP/sort.html) — 稳定的"快速排序"算法排序 （不推荐使用，见 gsort）

*   **线性代数[Linear Algebra](http://help.scilab.org/docs/5.4.0/ja_JP/section_3d664928f9e248b4bf1439a1e8bd3ef8.html)**

    *   [Eigenvalue and Singular Value](http://help.scilab.org/docs/5.4.0/ja_JP/section_f98e7b156394fdb45a775ce2595bf4b6.html)

            *   [balanc](http://help.scilab.org/docs/5.4.0/ja_JP/balanc.html) — 系统的矩阵或铅笔平衡
        *   [bdiag](http://help.scilab.org/docs/5.4.0/ja_JP/bdiag.html) — 块对角化，广义特征向量
        *   [gschur](http://help.scilab.org/docs/5.4.0/ja_JP/gschur.html) — 广义的 Schur 分解 （已过时）。
        *   [gspec](http://help.scilab.org/docs/5.4.0/ja_JP/gspec.html) — 特征值的矩阵铅笔 (已过时)
        *   [hess](http://help.scilab.org/docs/5.4.0/ja_JP/hess.html) — ヘッセンベルク形表达式
        *   [pbig](http://help.scilab.org/docs/5.4.0/ja_JP/pbig.html) — 自然投影
        *   [projspec](http://help.scilab.org/docs/5.4.0/ja_JP/projspec.html) — 光谱运算符
        *   [psmall](http://help.scilab.org/docs/5.4.0/ja_JP/psmall.html) — 光谱投影
        *   [schur](http://help.scilab.org/docs/5.4.0/ja_JP/schur.html) — Schur 分解的矩阵和铅笔 [排序]
        *   [spec](http://help.scilab.org/docs/5.4.0/ja_JP/spec.html) — 特征值的矩阵和铅笔
        *   [sva](http://help.scilab.org/docs/5.4.0/ja_JP/sva.html) — 奇异值逼近
        *   [svd](http://help.scilab.org/docs/5.4.0/ja_JP/svd.html) — 奇异值分解

        *   [Factorization](http://help.scilab.org/docs/5.4.0/ja_JP/section_502e3804d3e7f50dbf5f362b99f2cb78.html)

            *   [givens](http://help.scilab.org/docs/5.4.0/ja_JP/givens.html) — 吉文斯转型
        *   [householder](http://help.scilab.org/docs/5.4.0/ja_JP/householder.html) — 田主正交镜像反射矩阵
        *   [sqroot](http://help.scilab.org/docs/5.4.0/ja_JP/sqroot.html) — W ＊ W ' 厄米特分解

        *   [Kernel](http://help.scilab.org/docs/5.4.0/ja_JP/section_7478db78e01da53491132769fe3f29cb.html)

            *   [colcomp](http://help.scilab.org/docs/5.4.0/ja_JP/colcomp.html) — 列压缩、 内核、 nullspace
        *   [fullrf](http://help.scilab.org/docs/5.4.0/ja_JP/fullrf.html) — 满秩分解
        *   [fullrfk](http://help.scilab.org/docs/5.4.0/ja_JP/fullrfk.html) — A ^ k 满秩分解
        *   [im_inv](http://help.scilab.org/docs/5.4.0/ja_JP/im_inv.html) — 原始图像
        *   [kernel](http://help.scilab.org/docs/5.4.0/ja_JP/kernel.html) — 内核 nullspace
        *   [range](http://help.scilab.org/docs/5.4.0/ja_JP/range.html) — A ^ k 系列
        *   [rowcomp](http://help.scilab.org/docs/5.4.0/ja_JP/rowcomp.html) — 行压缩范围

        *   [Linear Equations](http://help.scilab.org/docs/5.4.0/ja_JP/section_bbfc3f7583f2a23ca6c78964d94d0456.html)

            *   [aff2ab](http://help.scilab.org/docs/5.4.0/ja_JP/aff2ab.html) — 线性 （仿） 的函数，将转换为 A，b
        *   [chol](http://help.scilab.org/docs/5.4.0/ja_JP/chol.html) — 乔莱斯基分解
        *   [inv](http://help.scilab.org/docs/5.4.0/ja_JP/inv.html) — 矩阵的逆矩阵
        *   [linsolve](http://help.scilab.org/docs/5.4.0/ja_JP/linsolve.html) — 线性方程求解
        *   [lsq](http://help.scilab.org/docs/5.4.0/ja_JP/lsq.html) — 线性最小二乘问题。
        *   [lu](http://help.scilab.org/docs/5.4.0/ja_JP/lu.html) — 选择数据透视表的 LU 分解
        *   [pinv](http://help.scilab.org/docs/5.4.0/ja_JP/pinv.html) — 广义的逆
        *   [qr](http://help.scilab.org/docs/5.4.0/ja_JP/qr.html) — QR 分解
        *   [rankqr](http://help.scilab.org/docs/5.4.0/ja_JP/rankqr.html) — 基于 QR 分解的秩

        *   [Markov Matrices](http://help.scilab.org/docs/5.4.0/ja_JP/section_7b64801bed20d50da59555f7221038e3.html)

            *   [classmarkov](http://help.scilab.org/docs/5.4.0/ja_JP/classmarkov.html) — 递归马尔可夫矩阵 （经常） 和临时 (瞬态) 一类
        *   [eigenmarkov](http://help.scilab.org/docs/5.4.0/ja_JP/eigenmarkov.html) — 归一化左和右马氏的特征向量
        *   [genmarkov](http://help.scilab.org/docs/5.4.0/ja_JP/genmarkov.html) — 生成随机马尔可夫矩阵的递归和一个临时类

        *   [Matrix Analysis](http://help.scilab.org/docs/5.4.0/ja_JP/section_37f17146f5835dea49507f7f7b476b59.html)

            *   [cond](http://help.scilab.org/docs/5.4.0/ja_JP/cond.html) — 条件数
        *   [det](http://help.scilab.org/docs/5.4.0/ja_JP/det.html) — 矩阵行列式
        *   [orth](http://help.scilab.org/docs/5.4.0/ja_JP/orth.html) — 正交基
        *   [rank](http://help.scilab.org/docs/5.4.0/ja_JP/rank.html) — 故事数量
        *   [rcond](http://help.scilab.org/docs/5.4.0/ja_JP/rcond.html) — 条件数倒数
        *   [rref](http://help.scilab.org/docs/5.4.0/ja_JP/rref.html) — LU 分解法计算矩阵行梯队形式
        *   [trace](http://help.scilab.org/docs/5.4.0/ja_JP/trace.html) — 跟踪

        *   [Matrix Pencil](http://help.scilab.org/docs/5.4.0/ja_JP/section_43390de3f16a72ac21f6707dcee73a6c.html)

            *   [companion](http://help.scilab.org/docs/5.4.0/ja_JP/companion.html) — 伴随矩阵
        *   [ereduc](http://help.scilab.org/docs/5.4.0/ja_JP/ereduc.html) — 通过 qz 转换计算楼梯列矩阵
        *   [fstair](http://help.scilab.org/docs/5.4.0/ja_JP/fstair.html) — 通过 qz 转换计算列形楼梯铅笔
        *   [glever](http://help.scilab.org/docs/5.4.0/ja_JP/glever.html) — 逆的矩阵铅笔
        *   [kroneck](http://help.scilab.org/docs/5.4.0/ja_JP/kroneck.html) — クロネッカー形表达的矩阵铅笔
        *   [lyap](http://help.scilab.org/docs/5.4.0/ja_JP/lyap.html) — 李雅普诺夫方程
        *   [pencan](http://help.scilab.org/docs/5.4.0/ja_JP/pencan.html) — 正矩阵铅笔关联窗体
        *   [penlaur](http://help.scilab.org/docs/5.4.0/ja_JP/penlaur.html) — 洛朗 · 系数的矩阵铅笔
        *   [quaskro](http://help.scilab.org/docs/5.4.0/ja_JP/quaskro.html) — 窗体准-克罗内克
        *   [randpencil](http://help.scilab.org/docs/5.4.0/ja_JP/randpencil.html) — 随机铅笔
        *   [rowshuff](http://help.scilab.org/docs/5.4.0/ja_JP/rowshuff.html) — 无序播放算法
        *   [sylv](http://help.scilab.org/docs/5.4.0/ja_JP/sylv.html) — 西尔维斯特方程。

        *   [State-Space Matrices](http://help.scilab.org/docs/5.4.0/ja_JP/section_843ad62b11fa0b298343f7f7701e205c.html)

            *   [coff](http://help.scilab.org/docs/5.4.0/ja_JP/coff.html) — 解决方案 (残余因素法)
        *   [nlev](http://help.scilab.org/docs/5.4.0/ja_JP/nlev.html) — Leverrier 的算法

        *   [Subspaces](http://help.scilab.org/docs/5.4.0/ja_JP/section_ad0675cb0e77c263d4d4b5fae27def76.html)

            *   [spaninter](http://help.scilab.org/docs/5.4.0/ja_JP/spaninter.html) — 常见的子空间
        *   [spanplus](http://help.scilab.org/docs/5.4.0/ja_JP/spanplus.html) — 子空间的总和
        *   [spantwo](http://help.scilab.org/docs/5.4.0/ja_JP/spantwo.html) — 交集和子空间的总和

        *   [proj](http://help.scilab.org/docs/5.4.0/ja_JP/proj.html) — 投影

*   **插值[Interpolation](http://help.scilab.org/docs/5.4.0/ja_JP/section_b9661dd1d4b7bb411d6af177310b6983.html)**

    *   [bsplin3val](http://help.scilab.org/docs/5.4.0/ja_JP/bsplin3val.html) — 3D 样条任意鉴别标准
    *   [cshep2d](http://help.scilab.org/docs/5.4.0/ja_JP/cshep2d.html) — 2D 3 以下谢泼德 （散点） 插值
    *   [eval_cshep2d](http://help.scilab.org/docs/5.4.0/ja_JP/eval_cshep2d.html) — 两个三维立方谢泼德插值评价
    *   [interp](http://help.scilab.org/docs/5.4.0/ja_JP/interp.html) — 三次样条插值
    *   [interp1](http://help.scilab.org/docs/5.4.0/ja_JP/interp1.html) — 1-维插值函数
    *   [interp2d](http://help.scilab.org/docs/5.4.0/ja_JP/interp2d.html) — (2D) 双三次样条插值
    *   [interp3d](http://help.scilab.org/docs/5.4.0/ja_JP/interp3d.html) — 3D三次样条插值
    *   [interpln](http://help.scilab.org/docs/5.4.0/ja_JP/interpln.html) — 线性插值
    *   [linear_interpn](http://help.scilab.org/docs/5.4.0/ja_JP/linear_interpn.html) — n 维线性插值
    *   [lsq_splin](http://help.scilab.org/docs/5.4.0/ja_JP/lsq_splin.html) — 加权的最小二乘三次样条
    *   [smooth](http://help.scilab.org/docs/5.4.0/ja_JP/smooth.html) — 平滑的样条函数
    *   [splin](http://help.scilab.org/docs/5.4.0/ja_JP/splin.html) — 计算三次样条插值需要的导数
    *   [splin2d](http://help.scilab.org/docs/5.4.0/ja_JP/splin2d.html) — 双立方样条网格的二维插值
    *   [splin3d](http://help.scilab.org/docs/5.4.0/ja_JP/splin3d.html) — 3 维插值样条网格

*   计算机辅助控制系统设计[CACSD](http://help.scilab.org/docs/5.4.0/ja_JP/section_d8d125e80c244a8a6f5869182481e3b9.html)

    *   [Format representations and conversions](http://help.scilab.org/docs/5.4.0/ja_JP/section_922b4248e57888297202afc5a6437172.html)

            *   [abcd](http://help.scilab.org/docs/5.4.0/ja_JP/abcd.html) — 状态空间矩阵
        *   [cont_frm](http://help.scilab.org/docs/5.4.0/ja_JP/cont_frm.html) — 可控状态空间转换
        *   [dbphi](http://help.scilab.org/docs/5.4.0/ja_JP/dbphi.html) — 振幅和相位的频率响应的表示形式
        *   [des2ss](http://help.scilab.org/docs/5.4.0/ja_JP/des2ss.html) — 从描述符状态空间
        *   [des2tf](http://help.scilab.org/docs/5.4.0/ja_JP/des2tf.html) — 因为要传输函数转换说明符
        *   [frep2tf](http://help.scilab.org/docs/5.4.0/ja_JP/frep2tf.html) — Get 从频率响应的传输功能实现
        *   [markp2ss](http://help.scilab.org/docs/5.4.0/ja_JP/markp2ss.html) — 转换为状态空间马尔可夫参数
        *   [sm2des](http://help.scilab.org/docs/5.4.0/ja_JP/sm2des.html) — 系统矩阵转换描述符
        *   [sm2ss](http://help.scilab.org/docs/5.4.0/ja_JP/sm2ss.html) — 将系统矩阵转换为状态空间
        *   [ss2des](http://help.scilab.org/docs/5.4.0/ja_JP/ss2des.html) — (多项式） 转换为状态空间描述符格式
        *   [ss2ss](http://help.scilab.org/docs/5.4.0/ja_JP/ss2ss.html) — 从状态到状态空间转换、 反馈、 注射
        *   [ss2tf](http://help.scilab.org/docs/5.4.0/ja_JP/ss2tf.html) — 状态空间传输函数转换
        *   [tf2des](http://help.scilab.org/docs/5.4.0/ja_JP/tf2des.html) — 成描述符的格式传递函数
        *   [tf2ss](http://help.scilab.org/docs/5.4.0/ja_JP/tf2ss.html) — 从传递函数转换为状态空间表示形式

        *   [Plot and display](http://help.scilab.org/docs/5.4.0/ja_JP/section_75c09d3a94a90a77a955f85ddaefc478.html)

            *   [black](http://help.scilab.org/docs/5.4.0/ja_JP/black.html) — 黑图 (Nichols 情节)
        *   [bode](http://help.scilab.org/docs/5.4.0/ja_JP/bode.html) — 博德阴谋
        *   [chart](http://help.scilab.org/docs/5.4.0/ja_JP/chart.html) — Nichols 情节的轮廓情节
        *   [evans](http://help.scilab.org/docs/5.4.0/ja_JP/evans.html) — 埃文斯根轨迹
        *   [gainplot](http://help.scilab.org/docs/5.4.0/ja_JP/gainplot.html) — 增益阴谋
        *   [hallchart](http://help.scilab.org/docs/5.4.0/ja_JP/hallchart.html) — 画馆
        *   [m_circle](http://help.scilab.org/docs/5.4.0/ja_JP/m_circle.html) — y / (y 1)，增益复杂平面绘制的轮廓
        *   [nicholschart](http://help.scilab.org/docs/5.4.0/ja_JP/nicholschart.html) — Nichols 阴谋
        *   [nyquist](http://help.scilab.org/docs/5.4.0/ja_JP/nyquist.html) — 奈奎斯特图
        *   [phaseplot](http://help.scilab.org/docs/5.4.0/ja_JP/phaseplot.html) — 频率和相位阴谋
        *   [sgrid](http://help.scilab.org/docs/5.4.0/ja_JP/sgrid.html) — s-平面网格线。
        *   [show_margins](http://help.scilab.org/docs/5.4.0/ja_JP/show_margins.html) — 获得边距和阶段的边距和交叉频率，每个节目
        *   [svplot](http://help.scilab.org/docs/5.4.0/ja_JP/svplot.html) — 奇异值西格玛阴谋
        *   [zgrid](http://help.scilab.org/docs/5.4.0/ja_JP/zgrid.html) — zgrid 地块

        *   [abinv](http://help.scilab.org/docs/5.4.0/ja_JP/abinv.html) — AB 不变子空间
    *   [arhnk](http://help.scilab.org/docs/5.4.0/ja_JP/arhnk.html) — ハンケルノルム 逼近
    *   [arl2](http://help.scilab.org/docs/5.4.0/ja_JP/arl2.html) — L2 转让逼近 SISO 模型实现
    *   [arma](http://help.scilab.org/docs/5.4.0/ja_JP/arma.html) — Scilab arma 库
    *   [arma2p](http://help.scilab.org/docs/5.4.0/ja_JP/arma2p.html) — 展开从 ar 的多项式矩阵
    *   [arma2ss](http://help.scilab.org/docs/5.4.0/ja_JP/arma2ss.html) — armax 状态空间表示形式转换为数据结构。
    *   [armac](http://help.scilab.org/docs/5.4.0/ja_JP/armac.html) — Scilab armax 过程的说明
    *   [armax](http://help.scilab.org/docs/5.4.0/ja_JP/armax.html) — ARMAX 鉴定
    *   [armax1](http://help.scilab.org/docs/5.4.0/ja_JP/armax1.html) — ARMAX 鉴定
    *   [arsimul](http://help.scilab.org/docs/5.4.0/ja_JP/arsimul.html) — ARMAX 仿真
    *   [augment](http://help.scilab.org/docs/5.4.0/ja_JP/augment.html) — 延长植物
    *   [balreal](http://help.scilab.org/docs/5.4.0/ja_JP/balreal.html) — 平衡的实现
    *   [bilin](http://help.scilab.org/docs/5.4.0/ja_JP/bilin.html) — 广义双线性双线性变换
    *   [bstap](http://help.scilab.org/docs/5.4.0/ja_JP/bstap.html) — 汉克尔逼近
    *   [cainv](http://help.scilab.org/docs/5.4.0/ja_JP/cainv.html) — 双重的 abinv
    *   [calfrq](http://help.scilab.org/docs/5.4.0/ja_JP/calfrq.html) — 频率响应的离散
    *   [canon](http://help.scilab.org/docs/5.4.0/ja_JP/canon.html) — 可制御正準形
    *   [ccontrg](http://help.scilab.org/docs/5.4.0/ja_JP/ccontrg.html) — H-无限控制器的集中解决方案
    *   [cls2dls](http://help.scilab.org/docs/5.4.0/ja_JP/cls2dls.html) — 双线性变换
    *   [colinout](http://help.scilab.org/docs/5.4.0/ja_JP/colinout.html) — インナアウタ 分解
    *   [colregul](http://help.scilab.org/docs/5.4.0/ja_JP/colregul.html) — 要除去杆和零到无穷大
    *   [cont_mat](http://help.scilab.org/docs/5.4.0/ja_JP/cont_mat.html) — 能控性矩阵
    *   [contr](http://help.scilab.org/docs/5.4.0/ja_JP/contr.html) — 可控性、 可控的子空间楼梯
    *   [contrss](http://help.scilab.org/docs/5.4.0/ja_JP/contrss.html) — 控制部件
    *   [copfac](http://help.scilab.org/docs/5.4.0/ja_JP/copfac.html) — 右互质因子分解
    *   [csim](http://help.scilab.org/docs/5.4.0/ja_JP/csim.html) — （响应时间） 线性系统的仿真
    *   [ctr_gram](http://help.scilab.org/docs/5.4.0/ja_JP/ctr_gram.html) — Gramian 可控性
    *   [damp](http://help.scilab.org/docs/5.4.0/ja_JP/damp.html) — 固有频率和阻尼乘数。
    *   [dcf](http://help.scilab.org/docs/5.4.0/ja_JP/dcf.html) — 双互质分解
    *   [ddp](http://help.scilab.org/docs/5.4.0/ja_JP/ddp.html) — 干扰解耦
    *   [dhinf](http://help.scilab.org/docs/5.4.0/ja_JP/dhinf.html) — H 无穷大的离散时间系统的设计
    *   [dhnorm](http://help.scilab.org/docs/5.4.0/ja_JP/dhnorm.html) — 离散 H 无穷范
    *   [dscr](http://help.scilab.org/docs/5.4.0/ja_JP/dscr.html) — 线性系统的离散化
    *   [dsimul](http://help.scilab.org/docs/5.4.0/ja_JP/dsimul.html) — 离散状态空间模拟
    *   [dt_ility](http://help.scilab.org/docs/5.4.0/ja_JP/dt_ility.html) — -检测测试
    *   [dtsi](http://help.scilab.org/docs/5.4.0/ja_JP/dtsi.html) — 非稳定的稳定分解
    *   [equil](http://help.scilab.org/docs/5.4.0/ja_JP/equil.html) — 对对称矩阵的平衡
    *   [equil1](http://help.scilab.org/docs/5.4.0/ja_JP/equil1.html) — 均衡矩阵 (非负正定) 一套
    *   [feedback](http://help.scilab.org/docs/5.4.0/ja_JP/feedback.html) — 反馈操作
    *   [findABCD](http://help.scilab.org/docs/5.4.0/ja_JP/findABCD.html) — 离散时间系统子空间辨识
    *   [findAC](http://help.scilab.org/docs/5.4.0/ja_JP/findAC.html) — 离散时间系统子空间辨识
    *   [findBD](http://help.scilab.org/docs/5.4.0/ja_JP/findBD.html) — 初始值和离散时间系统的系统矩阵 B 和 D 的状态
    *   [findBDK](http://help.scilab.org/docs/5.4.0/ja_JP/findBDK.html) — D 系统矩阵 b 卡尔曼和离散时间系统
    *   [findR](http://help.scilab.org/docs/5.4.0/ja_JP/findR.html) — 当您指定的矩阵的线性时不变系统预处理器
    *   [findx0BD](http://help.scilab.org/docs/5.4.0/ja_JP/findx0BD.html) — 估计的状态、 离散时间系统 B 和 D 矩阵
    *   [flts](http://help.scilab.org/docs/5.4.0/ja_JP/flts.html) — 响应时间 （离散时间、 采样的系统）
    *   [fourplan](http://help.scilab.org/docs/5.4.0/ja_JP/fourplan.html) — 扩展进厂到四种植物
    *   [freq](http://help.scilab.org/docs/5.4.0/ja_JP/freq.html) — 频率响应
    *   [freson](http://help.scilab.org/docs/5.4.0/ja_JP/freson.html) — 峰值频率
    *   [fspecg](http://help.scilab.org/docs/5.4.0/ja_JP/fspecg.html) — 稳定因式分解
    *   [fstabst](http://help.scilab.org/docs/5.4.0/ja_JP/fstabst.html) — 尤拉 (悠乐天) 和参数化
    *   [g_margin](http://help.scilab.org/docs/5.4.0/ja_JP/g_margin.html) — 增益和增益穿越频率
    *   [gamitg](http://help.scilab.org/docs/5.4.0/ja_JP/gamitg.html) — H-无限大型伽玛迭代
    *   [gcare](http://help.scilab.org/docs/5.4.0/ja_JP/gcare.html) — 控制黎卡提方程
    *   [gfare](http://help.scilab.org/docs/5.4.0/ja_JP/gfare.html) — フィルタリカッチ 方程
    *   [gfrancis](http://help.scilab.org/docs/5.4.0/ja_JP/gfrancis.html) — 弗朗西斯方程的跟踪
    *   [gtild](http://help.scilab.org/docs/5.4.0/ja_JP/gtild.html) — 颚化符操作
    *   [h2norm](http://help.scilab.org/docs/5.4.0/ja_JP/h2norm.html) — H2 规范
    *   [h_cl](http://help.scilab.org/docs/5.4.0/ja_JP/h_cl.html) — 闭环矩阵
    *   [h_inf](http://help.scilab.org/docs/5.4.0/ja_JP/h_inf.html) — H 无穷大 （中心） 控制器
    *   [h_inf_st](http://help.scilab.org/docs/5.4.0/ja_JP/h_inf_st.html) — 静态 H_infinity 问题
    *   [h_norm](http://help.scilab.org/docs/5.4.0/ja_JP/h_norm.html) — H 无穷范
    *   [hankelsv](http://help.scilab.org/docs/5.4.0/ja_JP/hankelsv.html) — 汉克尔奇异值
    *   [hinf](http://help.scilab.org/docs/5.4.0/ja_JP/hinf.html) — H 无穷大的连续时间系统的设计
    *   [imrep2ss](http://help.scilab.org/docs/5.4.0/ja_JP/imrep2ss.html) — 脉冲响应的状态空间实现
    *   [inistate](http://help.scilab.org/docs/5.4.0/ja_JP/inistate.html) — 初始价值的离散时间系统的状态估计
    *   [invsyslin](http://help.scilab.org/docs/5.4.0/ja_JP/invsyslin.html) — 逆系统
    *   [kpure](http://help.scilab.org/docs/5.4.0/ja_JP/kpure.html) — 连续 SISO 系统限制反馈增益
    *   [krac2](http://help.scilab.org/docs/5.4.0/ja_JP/krac2.html) — 反馈增益连续 SISO 系统限制
    *   [lcf](http://help.scilab.org/docs/5.4.0/ja_JP/lcf.html) — 归一化互质因子分解
    *   [leqr](http://help.scilab.org/docs/5.4.0/ja_JP/leqr.html) — H-无穷大 LQ 增益 （完整状态）
    *   [lft](http://help.scilab.org/docs/5.4.0/ja_JP/lft.html) — 分式线性变换
    *   [lin](http://help.scilab.org/docs/5.4.0/ja_JP/lin.html) — 线性化
    *   [linf](http://help.scilab.org/docs/5.4.0/ja_JP/linf.html) — 无穷范
    *   [linfn](http://help.scilab.org/docs/5.4.0/ja_JP/linfn.html) — 无穷范
    *   [linmeq](http://help.scilab.org/docs/5.4.0/ja_JP/linmeq.html) — 西尔维斯特和李雅普诺夫方程求解
    *   [lqe](http://help.scilab.org/docs/5.4.0/ja_JP/lqe.html) — 线性二次型估计 （卡尔曼滤波）
    *   [lqg](http://help.scilab.org/docs/5.4.0/ja_JP/lqg.html) — LQG 补偿器
    *   [lqg2stan](http://help.scilab.org/docs/5.4.0/ja_JP/lqg2stan.html) — 将 LQG 转换为标准的问题
    *   [lqg_ltr](http://help.scilab.org/docs/5.4.0/ja_JP/lqg_ltr.html) — LQG/LTR （循环变换恢复） 设计
    *   [lqr](http://help.scilab.org/docs/5.4.0/ja_JP/lqr.html) — LQ 补偿器 （完整状态）
    *   [ltitr](http://help.scilab.org/docs/5.4.0/ja_JP/ltitr.html) — 离散时间响应 (状态空间)
    *   [macglov](http://help.scilab.org/docs/5.4.0/ja_JP/macglov.html) — Mac Farlane · 格洛弗问题
    *   [minreal](http://help.scilab.org/docs/5.4.0/ja_JP/minreal.html) — 最小平衡的实现
    *   [minss](http://help.scilab.org/docs/5.4.0/ja_JP/minss.html) — 最小实现
    *   [mucomp](http://help.scilab.org/docs/5.4.0/ja_JP/mucomp.html) — 亩 (结构奇异值)
    *   [narsimul](http://help.scilab.org/docs/5.4.0/ja_JP/narsimul.html) — ARMAX 仿真 （使用 rtitr）
    *   [nehari](http://help.scilab.org/docs/5.4.0/ja_JP/nehari.html) — ネハリ 逼近
    *   [noisegen](http://help.scilab.org/docs/5.4.0/ja_JP/noisegen.html) — 噪声的产生
    *   [nyquistfrequencybounds](http://help.scilab.org/docs/5.4.0/ja_JP/nyquistfrequencybounds.html) — 若要计算到指定的奈奎斯特轨迹和出频率的矩形的频率。
    *   [obs_gram](http://help.scilab.org/docs/5.4.0/ja_JP/obs_gram.html) — Gramian 可观测性
    *   [obscont](http://help.scilab.org/docs/5.4.0/ja_JP/obscont.html) — 基于观测器的控制器
    *   [observer](http://help.scilab.org/docs/5.4.0/ja_JP/observer.html) — 观测器设计
    *   [obsv_mat](http://help.scilab.org/docs/5.4.0/ja_JP/obsv_mat.html) — 可观测性矩阵
    *   [obsvss](http://help.scilab.org/docs/5.4.0/ja_JP/obsvss.html) — 该可观测对象的一部分
    *   [p_margin](http://help.scilab.org/docs/5.4.0/ja_JP/p_margin.html) — 相交叉频率和相位裕度
    *   [parrot](http://help.scilab.org/docs/5.4.0/ja_JP/parrot.html) — 鹦鹉的问题
    *   [pfss](http://help.scilab.org/docs/5.4.0/ja_JP/pfss.html) — 部分分解
    *   [phasemag](http://help.scilab.org/docs/5.4.0/ja_JP/phasemag.html) — 相位和振幅的计算
    *   [pol2des](http://help.scilab.org/docs/5.4.0/ja_JP/pol2des.html) — 多项式矩阵表示法
    *   [ppol](http://help.scilab.org/docs/5.4.0/ja_JP/ppol.html) — 极点配置
    *   [prbs_a](http://help.scilab.org/docs/5.4.0/ja_JP/prbs_a.html) — 生成的伪随机二进制数
    *   [projsl](http://help.scilab.org/docs/5.4.0/ja_JP/projsl.html) — 线性系统投影
    *   [reglin](http://help.scilab.org/docs/5.4.0/ja_JP/reglin.html) — 线性回归
    *   [repfreq](http://help.scilab.org/docs/5.4.0/ja_JP/repfreq.html) — 频率响应
    *   [ric_desc](http://help.scilab.org/docs/5.4.0/ja_JP/ric_desc.html) — 黎卡提方程
    *   [ricc](http://help.scilab.org/docs/5.4.0/ja_JP/ricc.html) — 黎卡提方程
    *   [riccati](http://help.scilab.org/docs/5.4.0/ja_JP/riccati.html) — 黎卡提方程
    *   [routh_t](http://help.scilab.org/docs/5.4.0/ja_JP/routh_t.html) — 劳斯表
    *   [rowinout](http://help.scilab.org/docs/5.4.0/ja_JP/rowinout.html) — 哪里-分解出
    *   [rowregul](http://help.scilab.org/docs/5.4.0/ja_JP/rowregul.html) — 无穷大移除杆和零
    *   [rtitr](http://help.scilab.org/docs/5.4.0/ja_JP/rtitr.html) — 离散时间响应 （转移矩阵）
    *   [sensi](http://help.scilab.org/docs/5.4.0/ja_JP/sensi.html) — 灵敏度功能
    *   [sident](http://help.scilab.org/docs/5.4.0/ja_JP/sident.html) — 卡尔曼增益与离散状态空间实现
    *   [sorder](http://help.scilab.org/docs/5.4.0/ja_JP/sorder.html) — 计算离散时间系统的程度
    *   [specfact](http://help.scilab.org/docs/5.4.0/ja_JP/specfact.html) — 谱分解
    *   [ssprint](http://help.scilab.org/docs/5.4.0/ja_JP/ssprint.html) — 线性系统的格式化输出
    *   [st_ility](http://help.scilab.org/docs/5.4.0/ja_JP/st_ility.html) — 稳定性测试
    *   [stabil](http://help.scilab.org/docs/5.4.0/ja_JP/stabil.html) — 镇定
    *   [sysfact](http://help.scilab.org/docs/5.4.0/ja_JP/sysfact.html) — 系统分解
    *   [syssize](http://help.scilab.org/docs/5.4.0/ja_JP/syssize.html) — 国家空间系统的大小
    *   [time_id](http://help.scilab.org/docs/5.4.0/ja_JP/time_id.html) — SISO 最小二乘识别
    *   [trzeros](http://help.scilab.org/docs/5.4.0/ja_JP/trzeros.html) — 传输零和正常秩
    *   [ui_observer](http://help.scilab.org/docs/5.4.0/ja_JP/ui_observer.html) — 未知输入观测器
    *   [unobs](http://help.scilab.org/docs/5.4.0/ja_JP/unobs.html) — 非观察空间
    *   [zeropen](http://help.scilab.org/docs/5.4.0/ja_JP/zeropen.html) — ゼロペンシル

*   **多项式[Polynomials](http://help.scilab.org/docs/5.4.0/ja_JP/section_cb7c89640a32bcf2b4b5c19b40d19568.html)**

    *   [bezout](http://help.scilab.org/docs/5.4.0/ja_JP/bezout.html) — H 总动物园的整数或多项式方程
    *   [cmndred](http://help.scilab.org/docs/5.4.0/ja_JP/cmndred.html) — 通用分母形表达式
    *   [coeff](http://help.scilab.org/docs/5.4.0/ja_JP/coeff.html) — 系数的多项式矩阵
    *   [coffg](http://help.scilab.org/docs/5.4.0/ja_JP/coffg.html) — 多项式矩阵的逆
    *   [colcompr](http://help.scilab.org/docs/5.4.0/ja_JP/colcompr.html) — 多项式矩阵的列压缩
    *   [degree](http://help.scilab.org/docs/5.4.0/ja_JP/degree.html) — 程度的多项式矩阵
    *   [denom](http://help.scilab.org/docs/5.4.0/ja_JP/denom.html) — 分母
    *   [derivat](http://help.scilab.org/docs/5.4.0/ja_JP/derivat.html) — 理性矩阵导数
    *   [determ](http://help.scilab.org/docs/5.4.0/ja_JP/determ.html) — 多项式矩阵的行列式值
    *   [detr](http://help.scilab.org/docs/5.4.0/ja_JP/detr.html) — 多项式的行列式
    *   [diophant](http://help.scilab.org/docs/5.4.0/ja_JP/diophant.html) — ダイオファンタイン (吃动物园) 方程
    *   [factors](http://help.scilab.org/docs/5.4.0/ja_JP/factors.html) — 实因式分解
    *   [hermit](http://help.scilab.org/docs/5.4.0/ja_JP/hermit.html) — エルミート形表达式
    *   [horner](http://help.scilab.org/docs/5.4.0/ja_JP/horner.html) — 评价的多项式 / 理性的数字
    *   [hrmt](http://help.scilab.org/docs/5.4.0/ja_JP/hrmt.html) — 多项式的最大公约数
    *   [htrianr](http://help.scilab.org/docs/5.4.0/ja_JP/htrianr.html) — Triangularization 的多项式矩阵
    *   [inv_coeff](http://help.scilab.org/docs/5.4.0/ja_JP/inv_coeff.html) — 因子的多项式矩阵
    *   [invr](http://help.scilab.org/docs/5.4.0/ja_JP/invr.html) — （合理） 的矩阵的逆
    *   [lcmdiag](http://help.scilab.org/docs/5.4.0/ja_JP/lcmdiag.html) — 最小公倍数对角线决议
    *   [ldiv](http://help.scilab.org/docs/5.4.0/ja_JP/ldiv.html) — 多项式矩阵长除法
    *   [numer](http://help.scilab.org/docs/5.4.0/ja_JP/numer.html) — 分子
    *   [pdiv](http://help.scilab.org/docs/5.4.0/ja_JP/pdiv.html) — 多项式司
    *   [pol2str](http://help.scilab.org/docs/5.4.0/ja_JP/pol2str.html) — 将多项式转换为字符串
    *   [polfact](http://help.scilab.org/docs/5.4.0/ja_JP/polfact.html) — 最小的因素
    *   [poly](http://help.scilab.org/docs/5.4.0/ja_JP/poly.html) — 要定义一个多项式
    *   [rational](http://help.scilab.org/docs/5.4.0/ja_JP/rational.html) — Scilab 对象，Scilab 有理数
    *   [residu](http://help.scilab.org/docs/5.4.0/ja_JP/residu.html) — 残值
    *   [roots](http://help.scilab.org/docs/5.4.0/ja_JP/roots.html) — 多项式的根
    *   [rowcompr](http://help.scilab.org/docs/5.4.0/ja_JP/rowcompr.html) — 多项式矩阵的行压缩
    *   [sfact](http://help.scilab.org/docs/5.4.0/ja_JP/sfact.html) — 离散时间谱分析
    *   [simp](http://help.scilab.org/docs/5.4.0/ja_JP/simp.html) — 合理简化
    *   [simp_mode](http://help.scilab.org/docs/5.4.0/ja_JP/simp_mode.html) — 打开/关闭开关的合理简化
    *   [sylm](http://help.scilab.org/docs/5.4.0/ja_JP/sylm.html) — 西尔维斯特 · 矩阵
    *   [systmat](http://help.scilab.org/docs/5.4.0/ja_JP/systmat.html) — 系统矩阵
    *   [varn](http://help.scilab.org/docs/5.4.0/ja_JP/varn.html) — 符号变量多项式

*   信号处理[Signal Processing](http://help.scilab.org/docs/5.4.0/ja_JP/section_21be3ee00689bb50494bba0d79a6585a.html)

    *   [filters](http://help.scilab.org/docs/5.4.0/ja_JP/section_385b64aaddc3af590c99c03ea9c476e0.html)

            *   [analpf](http://help.scilab.org/docs/5.4.0/ja_JP/analpf.html) — 若要创建通道过滤
        *   [buttmag](http://help.scilab.org/docs/5.4.0/ja_JP/buttmag.html) — 巴特沃斯滤波器的响应
        *   [casc](http://help.scilab.org/docs/5.4.0/ja_JP/casc.html) — 创建筛选器的级联的实现从系数
        *   [cheb1mag](http://help.scilab.org/docs/5.4.0/ja_JP/cheb1mag.html) — 切比雪夫 1 型筛选器的响应
        *   [cheb2mag](http://help.scilab.org/docs/5.4.0/ja_JP/cheb2mag.html) — 响应的类型 2 切比雪夫滤波器
        *   [chepol](http://help.scilab.org/docs/5.4.0/ja_JP/chepol.html) — 切比雪夫多项式
        *   [convol](http://help.scilab.org/docs/5.4.0/ja_JP/convol.html) — 卷积
        *   [ell1mag](http://help.scilab.org/docs/5.4.0/ja_JP/ell1mag.html) — 椭圆滤波器的规模
        *   [eqfir](http://help.scilab.org/docs/5.4.0/ja_JP/eqfir.html) — FIR 滤波器的极大极小逼近
        *   [eqiir](http://help.scilab.org/docs/5.4.0/ja_JP/eqiir.html) — IIR 滤波器设计
        *   [faurre](http://help.scilab.org/docs/5.4.0/ja_JP/faurre.html) — Faurre 算法计算的筛选器
        *   [ffilt](http://help.scilab.org/docs/5.4.0/ja_JP/ffilt.html) — FIR 低通滤波器的系数
        *   [filter](http://help.scilab.org/docs/5.4.0/ja_JP/filter.html) — 数字筛选器的筛选器处理的数据系列
        *   [find_freq](http://help.scilab.org/docs/5.4.0/ja_JP/find_freq.html) — 获取参数兼容的椭圆滤波器的设计
        *   [frmag](http://help.scilab.org/docs/5.4.0/ja_JP/frmag.html) — FIR 与 IIR 滤波器的规模
        *   [fsfirlin](http://help.scilab.org/docs/5.4.0/ja_JP/fsfirlin.html) — 杉木，线性相位滤波器频率采样方法 e 的设计
        *   [group](http://help.scilab.org/docs/5.4.0/ja_JP/group.html) — 数字滤波器的群延时
        *   [iir](http://help.scilab.org/docs/5.4.0/ja_JP/iir.html) — IIR 数字滤波器
        *   [iirgroup](http://help.scilab.org/docs/5.4.0/ja_JP/iirgroup.html) — IIR 滤波器组延迟 Lp 优化
        *   [iirlp](http://help.scilab.org/docs/5.4.0/ja_JP/iirlp.html) — LP IIR 滤波器优化
        *   [kalm](http://help.scilab.org/docs/5.4.0/ja_JP/kalm.html) — 卡尔曼更新
        *   [lev](http://help.scilab.org/docs/5.4.0/ja_JP/lev.html) — 尤尔-沃克方程 （列文森的算法）
        *   [levin](http://help.scilab.org/docs/5.4.0/ja_JP/levin.html) — (多维)求解 Toeplitz 系统的莱文森算法
        *   [lindquist](http://help.scilab.org/docs/5.4.0/ja_JP/lindquist.html) — 中的算法
        *   [remezb](http://help.scilab.org/docs/5.4.0/ja_JP/remezb.html) — 极大极小逼近的幅度响应
        *   [srfaur](http://help.scilab.org/docs/5.4.0/ja_JP/srfaur.html) — 平方根算法
        *   [srkf](http://help.scilab.org/docs/5.4.0/ja_JP/srkf.html) — 平方根卡尔曼滤波
        *   [sskf](http://help.scilab.org/docs/5.4.0/ja_JP/sskf.html) — 稳定状态卡尔曼滤波
        *   [system](http://help.scilab.org/docs/5.4.0/ja_JP/system.html) — 观察更新
        *   [trans](http://help.scilab.org/docs/5.4.0/ja_JP/trans.html) — 要转换为其他筛选器 rūpnagar
        *   [wfir](http://help.scilab.org/docs/5.4.0/ja_JP/wfir.html) — 线性相位 FIR 滤波器
        *   [wiener](http://help.scilab.org/docs/5.4.0/ja_JP/wiener.html) — 维纳估计
        *   [wigner](http://help.scilab.org/docs/5.4.0/ja_JP/wigner.html) — '时频' ウイナースペクトラム
        *   [window](http://help.scilab.org/docs/5.4.0/ja_JP/window.html) — 计算对称的各种类型的窗口
        *   [zpbutt](http://help.scilab.org/docs/5.4.0/ja_JP/zpbutt.html) — 巴特沃思模拟滤波器
        *   [zpch1](http://help.scilab.org/docs/5.4.0/ja_JP/zpch1.html) — 切比雪夫模拟滤波器
        *   [zpch2](http://help.scilab.org/docs/5.4.0/ja_JP/zpch2.html) — 切比雪夫模拟滤波器
        *   [zpell](http://help.scilab.org/docs/5.4.0/ja_JP/zpell.html) — 椭圆低通滤波器

        *   [How to](http://help.scilab.org/docs/5.4.0/ja_JP/section_fbaa10eb3453a01088841542152da4df.html)

            *   [DesignEllipticFilter](http://help.scilab.org/docs/5.4.0/ja_JP/DesignEllipticFilter.html) — 设计方法的椭圆滤波器 (模拟和数字）

        *   [identification](http://help.scilab.org/docs/5.4.0/ja_JP/section_a1211667a0a0ac45f121915ff67fae96.html)

            *   [lattn](http://help.scilab.org/docs/5.4.0/ja_JP/lattn.html) — 正常的方程的迭代解
        *   [lattp](http://help.scilab.org/docs/5.4.0/ja_JP/lattp.html) — lattp
        *   [phc](http://help.scilab.org/docs/5.4.0/ja_JP/phc.html) — 马氏代表性
        *   [rpem](http://help.scilab.org/docs/5.4.0/ja_JP/rpem.html) — 递推估计的最小值估计

        *   [miscellaneous](http://help.scilab.org/docs/5.4.0/ja_JP/section_d35c6f0da1dd0d5aaa3601e99cea892b.html)

            *   [bilt](http://help.scilab.org/docs/5.4.0/ja_JP/bilt.html) — SISO 系统的主或双二阶的零极点表示形式变换
        *   [jmat](http://help.scilab.org/docs/5.4.0/ja_JP/jmat.html) — 行或列块交换
        *   [sincd](http://help.scilab.org/docs/5.4.0/ja_JP/sincd.html) — 数字 sinc 函数或 Direchlet 内核

        *   [spectral_estimation](http://help.scilab.org/docs/5.4.0/ja_JP/section_ed4a8fad8ff58973fd1e0f90241a811e.html)

            *   [corr](http://help.scilab.org/docs/5.4.0/ja_JP/corr.html) — 相关性、 协方差
        *   [cspect](http://help.scilab.org/docs/5.4.0/ja_JP/cspect.html) — 两边相互之间关联法 2 离散时间信号的谱估计
        *   [czt](http://help.scilab.org/docs/5.4.0/ja_JP/czt.html) — 啁啾 z 变换算法
        *   [intdec](http://help.scilab.org/docs/5.4.0/ja_JP/intdec.html) — 更改信号的采样率
        *   [mese](http://help.scilab.org/docs/5.4.0/ja_JP/mese.html) — 最大熵谱估计
        *   [pspect](http://help.scilab.org/docs/5.4.0/ja_JP/pspect.html) — 韦尔奇的平均周期图法的离散时间信号之间的双面交叉谱估计......

        *   [transforms](http://help.scilab.org/docs/5.4.0/ja_JP/section_4fda8b1a542129bbfb319daf21121d2a.html)

            *   [dct](http://help.scilab.org/docs/5.4.0/ja_JP/dct.html) — 反离散余弦变换。
        *   [dft](http://help.scilab.org/docs/5.4.0/ja_JP/dft.html) — 离散傅里叶变换
        *   [dst](http://help.scilab.org/docs/5.4.0/ja_JP/dst.html) — 反离散正弦变换。
        *   [fft](http://help.scilab.org/docs/5.4.0/ja_JP/fft.html) — 快速傅里叶变换逆
        *   [hank](http://help.scilab.org/docs/5.4.0/ja_JP/hank.html) — 从向汉克尔矩阵协方差
        *   [hilb](http://help.scilab.org/docs/5.4.0/ja_JP/hilb.html) — 杉木逼近的救生员转换筛选器
        *   [mfft](http://help.scilab.org/docs/5.4.0/ja_JP/mfft.html) — 多维 FFT

        *   [cepstrum](http://help.scilab.org/docs/5.4.0/ja_JP/cepstrum.html) — 倒谱计算
    *   [conv](http://help.scilab.org/docs/5.4.0/ja_JP/conv.html) — 1 (D) 离散卷积
    *   [conv2](http://help.scilab.org/docs/5.4.0/ja_JP/conv2.html) — 离散的二维卷积。
    *   [convol2d](http://help.scilab.org/docs/5.4.0/ja_JP/convol2d.html) — 离散 2 d 包括折叠，使用 fft。
    *   [detrend](http://help.scilab.org/docs/5.4.0/ja_JP/detrend.html) — 从向量中删除常数、 线性或分段线性趋势
    *   [fft2](http://help.scilab.org/docs/5.4.0/ja_JP/fft2.html) — 2 维快速傅里叶变换
    *   [fftshift](http://help.scilab.org/docs/5.4.0/ja_JP/fftshift.html) — 重新排列的 fft 输出和通过光谱的中心频率 0
    *   [filt_sinc](http://help.scilab.org/docs/5.4.0/ja_JP/filt_sinc.html) — sinc 函数的样本
    *   [frfit](http://help.scilab.org/docs/5.4.0/ja_JP/frfit.html) — 适合的频率响应
    *   [hilbert](http://help.scilab.org/docs/5.4.0/ja_JP/hilbert.html) — 若要计算的真实世界信号的离散信号由救生员转换
    *   [mrfit](http://help.scilab.org/docs/5.4.0/ja_JP/mrfit.html) — 适合的频率响应
    *   [remez](http://help.scilab.org/docs/5.4.0/ja_JP/remez.html) — 雷米兹交换算法连续函数来求和余弦加权切比雪夫逼近。
    *   [syredi](http://help.scilab.org/docs/5.4.0/ja_JP/syredi.html) — Syredi 代码接口，IIR 滤波器的设计
    *   [wfir_gui](http://help.scilab.org/docs/5.4.0/ja_JP/wfir_gui.html) — 用于设计交互式 wfir 筛选器 GUI
    *   [xcorr](http://help.scilab.org/docs/5.4.0/ja_JP/xcorr.html) — 来计算离散的自相关
    *   [xcov](http://help.scilab.org/docs/5.4.0/ja_JP/xcov.html) — 要计算离散自我 / 交叉协方差
    *   [yulewalk](http://help.scilab.org/docs/5.4.0/ja_JP/yulewalk.html) — 最小平方滤波器设计

*   [FFTW](http://help.scilab.org/docs/5.4.0/ja_JP/section_fb4f9a568728676c8280b2765096f44e.html)

    *   [fftw](http://help.scilab.org/docs/5.4.0/ja_JP/fftw.html) — 基于 fftw 库的快速傅里叶变换
    *   [fftw_flags](http://help.scilab.org/docs/5.4.0/ja_JP/fftw_flags.html) — fftw 函数的快速傅里叶变换算法
    *   [fftw_forget_wisdom](http://help.scilab.org/docs/5.4.0/ja_JP/fftw_forget_wisdom.html) — 重置 fftw 智慧
    *   [get_fftw_wisdom](http://help.scilab.org/docs/5.4.0/ja_JP/get_fftw_wisdom.html) — 返回 fftw 智慧
    *   [set_fftw_wisdom](http://help.scilab.org/docs/5.4.0/ja_JP/set_fftw_wisdom.html) — 设置 fftw 的智慧

*   特殊函数[Special Functions](http://help.scilab.org/docs/5.4.0/ja_JP/section_34901b473753caffd1c14e17c2a39259.html)

    *   [amell](http://help.scilab.org/docs/5.4.0/ja_JP/amell.html) — 雅可比的 am 功能
    *   [bessel](http://help.scilab.org/docs/5.4.0/ja_JP/bessel.html) — （这是汉克尔函数相同） 贝塞尔函数的第二 3 物种
    *   [beta](http://help.scilab.org/docs/5.4.0/ja_JP/beta.html) — Beta 函数 （1 类欧拉积分)
    *   [calerf](http://help.scilab.org/docs/5.4.0/ja_JP/calerf.html) — 若要计算误差函数。
    *   [delip](http://help.scilab.org/docs/5.4.0/ja_JP/delip.html) — 类型完全和不完全椭圆积分
    *   [dlgamma](http://help.scilab.org/docs/5.4.0/ja_JP/dlgamma.html) — 伽玛函数，防扩散安全倡议函数的导数
    *   [erf](http://help.scilab.org/docs/5.4.0/ja_JP/erf.html) — 错误的函数。
    *   [erfc](http://help.scilab.org/docs/5.4.0/ja_JP/erfc.html) — 相位互补误差函数。
    *   [erfcx](http://help.scilab.org/docs/5.4.0/ja_JP/erfcx.html) — 与缩放互补误差函数。
    *   [erfinv](http://help.scilab.org/docs/5.4.0/ja_JP/erfinv.html) — 逆误差函数
    *   [findm](http://help.scilab.org/docs/5.4.0/ja_JP/findm.html) — 椭圆滤波器设计
    *   [gamma](http://help.scilab.org/docs/5.4.0/ja_JP/gamma.html) — 伽玛函数。
    *   [gammaln](http://help.scilab.org/docs/5.4.0/ja_JP/gammaln.html) — 伽玛函数的对数。
    *   [legendre](http://help.scilab.org/docs/5.4.0/ja_JP/legendre.html) — 相关勒让德函数
    *   [oldbessel](http://help.scilab.org/docs/5.4.0/ja_JP/oldbessel.html) — 第二类贝塞尔函数 (Y_alpha)。
    *   [percentasn](http://help.scilab.org/docs/5.4.0/ja_JP/percentasn.html) — 椭圆积分 l
    *   [percentk](http://help.scilab.org/docs/5.4.0/ja_JP/percentk.html) — 雅可比的完全椭圆积分
    *   [percentsn](http://help.scilab.org/docs/5.4.0/ja_JP/percentsn.html) — 雅可比椭圆函数

*   随机库[Randlib](http://help.scilab.org/docs/5.4.0/ja_JP/section_2482f7fcdef461e6bc215d5e0e564623.html)

    *   [grand](http://help.scilab.org/docs/5.4.0/ja_JP/grand.html) — 随机数生成器

*   [ARnoldi PACKage](http://help.scilab.org/docs/5.4.0/ja_JP/section_884b78bd769f63aed6b59d5fa748bbab.html)

    *   [dnaupd](http://help.scilab.org/docs/5.4.0/ja_JP/dnaupd.html) — 为隐式重新启动阿诺尔迪迭代，来计算这个函数是真正线性算子的几个特征对逼近过时的接口。 请使用 eigs
    *   [dneupd](http://help.scilab.org/docs/5.4.0/ja_JP/dneupd.html) — 接口为隐式重新启动阿诺尔迪迭代，计算 A 的特征值融合的近似 ＊ z = lambda ＊ B ＊ 这个函数是真正线性算子的几个特征对 z 逼近过时。 请使用 eigs
    *   [dsaupd](http://help.scilab.org/docs/5.4.0/ja_JP/dsaupd.html) — 接口为隐式重新启动阿诺尔迪迭代，来计算过时的几个特征对此函数是一个真正的和对称的线性算子的逼近。 请使用 eigs
    *   [dseupd](http://help.scilab.org/docs/5.4.0/ja_JP/dseupd.html) — 接口为隐式重新启动阿诺尔迪迭代，计算 A 的特征值融合近似逼近 ＊ z = lambda ＊ B ＊ z 此函数已过时。 请使用 eigs
    *   [eigs](http://help.scilab.org/docs/5.4.0/ja_JP/eigs.html) — 计算的特征值和特征向量的矩阵
    *   [znaupd](http://help.scilab.org/docs/5.4.0/ja_JP/znaupd.html) — 为隐式重新启动阿诺尔迪迭代，来计算复杂线性运算符 OP 就由厄米特半正定真正矩阵 B.定义双半内产品的几个特征对接口 此函数已过时。 请使用 eigs
    *   [zneupd](http://help.scilab.org/docs/5.4.0/ja_JP/zneupd.html) — 接口为隐式重新启动阿诺尔迪迭代，计算 A 的特征值融合近似逼近 ＊ z = lambda ＊ B ＊ z 此函数已过时。 请使用 eigs

*   **统计[Statistics](http://help.scilab.org/docs/5.4.0/ja_JP/section_64d0bca8a4d67a31e49865dd38a0415d.html)**

    *   [Cumulated Distribution Functions](http://help.scilab.org/docs/5.4.0/ja_JP/section_f88ebad645a3d646fdaa56b04ac4b5d4.html)

            *   [cdfbet](http://help.scilab.org/docs/5.4.0/ja_JP/cdfbet.html) — 累积分布函数测试版
        *   [cdfbin](http://help.scilab.org/docs/5.4.0/ja_JP/cdfbin.html) — 分布的累积分布函数 (2)
        *   [cdfchi](http://help.scilab.org/docs/5.4.0/ja_JP/cdfchi.html) — 累积分布函数： χ 2 分布
        *   [cdfchn](http://help.scilab.org/docs/5.4.0/ja_JP/cdfchn.html) — 累积分布函数： 非中心卡方分布
        *   [cdff](http://help.scilab.org/docs/5.4.0/ja_JP/cdff.html) — 累积分布函数： F 分布
        *   [cdffnc](http://help.scilab.org/docs/5.4.0/ja_JP/cdffnc.html) — 累积分布函数： 非中心的 F 分布
        *   [cdfgam](http://help.scilab.org/docs/5.4.0/ja_JP/cdfgam.html) — 累积分布函数： 伽玛分布
        *   [cdfnbn](http://help.scilab.org/docs/5.4.0/ja_JP/cdfnbn.html) — 累积分布函数： （2） 分布负
        *   [cdfnor](http://help.scilab.org/docs/5.4.0/ja_JP/cdfnor.html) — 累积分布函数： 正态分布
        *   [cdfpoi](http://help.scilab.org/docs/5.4.0/ja_JP/cdfpoi.html) — 累积分布函数： 泊松分布
        *   [cdft](http://help.scilab.org/docs/5.4.0/ja_JP/cdft.html) — 累积分布函数： 学生的 T 分布

        *   [Central Tendency](http://help.scilab.org/docs/5.4.0/ja_JP/section_f7d9d0bceb3f05f66ea6369f7a350f29.html)

            *   [geomean](http://help.scilab.org/docs/5.4.0/ja_JP/geomean.html) — 几何平均数
        *   [harmean](http://help.scilab.org/docs/5.4.0/ja_JP/harmean.html) — 调和平均值
        *   [mean](http://help.scilab.org/docs/5.4.0/ja_JP/mean.html) — 平均的向量 / 矩阵 （并行平均、 平均列）
        *   [meanf](http://help.scilab.org/docs/5.4.0/ja_JP/meanf.html) — 向量或矩阵的加权的平均
        *   [trimmean](http://help.scilab.org/docs/5.4.0/ja_JP/trimmean.html) — 裁切的均值的向量或矩阵

        *   [Data with Missing Values](http://help.scilab.org/docs/5.4.0/ja_JP/section_e0ff212af10e793483caef88824c699e.html)

            *   [nancumsum](http://help.scilab.org/docs/5.4.0/ja_JP/nancumsum.html) — 矩阵的值的累积总数
        *   [nand2mean](http://help.scilab.org/docs/5.4.0/ja_JP/nand2mean.html) — 两个独立的平均值之间的差异
        *   [nanmax](http://help.scilab.org/docs/5.4.0/ja_JP/nanmax.html) — （忽略 Nan） 的最大值
        *   [nanmean](http://help.scilab.org/docs/5.4.0/ja_JP/nanmean.html) — 意思是 （忽略 Nan）
        *   [nanmeanf](http://help.scilab.org/docs/5.4.0/ja_JP/nanmeanf.html) — 指定的频率平均值 （忽略 Nan）。
        *   [nanmedian](http://help.scilab.org/docs/5.4.0/ja_JP/nanmedian.html) — 中值的数值向量或矩阵
        *   [nanmin](http://help.scilab.org/docs/5.4.0/ja_JP/nanmin.html) — （忽略 Nan） 的最小值
        *   [nanstdev](http://help.scilab.org/docs/5.4.0/ja_JP/nanstdev.html) — （忽略 NaN） 的标准偏差。
        *   [nansum](http://help.scilab.org/docs/5.4.0/ja_JP/nansum.html) — NaN，值的总和
        *   [thrownan](http://help.scilab.org/docs/5.4.0/ja_JP/thrownan.html) — 删除 NaN 值

        *   [Descriptive Statistics](http://help.scilab.org/docs/5.4.0/ja_JP/section_bd910fc34bc5bef28579869077745722.html)

            *   [center](http://help.scilab.org/docs/5.4.0/ja_JP/center.html) — 中心
        *   [correl](http://help.scilab.org/docs/5.4.0/ja_JP/correl.html) — 计算两个变量之间的线性相关系数（皮尔逊积差系数 两个变量协方差除以两个变量的标准差）
        *   [covar](http://help.scilab.org/docs/5.4.0/ja_JP/covar.html) — 两个变量的协方差
        *   [median](http://help.scilab.org/docs/5.4.0/ja_JP/median.html) — 位数 （行中位数，每列中的值，......） 的向量 / 矩阵 / 阵列元素
        *   [msd](http://help.scilab.org/docs/5.4.0/ja_JP/msd.html) — 标准差（均方差）sqrt(方差/N)
        *   [mvvacov](http://help.scilab.org/docs/5.4.0/ja_JP/mvvacov.html) — 分布式-计算协方差矩阵
        *   [st_deviation](http://help.scilab.org/docs/5.4.0/ja_JP/st_deviation.html) — 标准偏差 sqrt(方差/(N-1) )
        *   [stdevf](http://help.scilab.org/docs/5.4.0/ja_JP/stdevf.html) — 带计数向量的标准偏差 sqrt(方差/(N-1) )
        *   [variance](http://help.scilab.org/docs/5.4.0/ja_JP/variance.html) — 向量或矩阵的值分布
        *   [variancef](http://help.scilab.org/docs/5.4.0/ja_JP/variancef.html) — 向量或矩阵的值的标准偏差
        *   [wcenter](http://help.scilab.org/docs/5.4.0/ja_JP/wcenter.html) — 加权质心和

        *   [Hypothesis Testing](http://help.scilab.org/docs/5.4.0/ja_JP/section_a2db718e75ccadd9377d47d9e01fc54c.html)

            *   [ftest](http://help.scilab.org/docs/5.4.0/ja_JP/ftest.html) — 菲舍尔比率
        *   [ftuneq](http://help.scilab.org/docs/5.4.0/ja_JP/ftuneq.html) — 样本大小不等于 Fisher 比率。

        *   [Measures of Dispersion](http://help.scilab.org/docs/5.4.0/ja_JP/section_1e97676f5286c23dcf85de2ea2f2270e.html)

            *   [iqr](http://help.scilab.org/docs/5.4.0/ja_JP/iqr.html) — 是四分位数的范围
        *   [mad](http://help.scilab.org/docs/5.4.0/ja_JP/mad.html) — 平均绝对偏差
        *   [strange](http://help.scilab.org/docs/5.4.0/ja_JP/strange.html) — 范围

        *   [Measures of Shape](http://help.scilab.org/docs/5.4.0/ja_JP/section_8f6a15a68846281dd4c07e319c83c88f.html)

            *   [cmoment](http://help.scilab.org/docs/5.4.0/ja_JP/cmoment.html) — 所有订单的中心矩
        *   [moment](http://help.scilab.org/docs/5.4.0/ja_JP/moment.html) — 鉴于非中央时刻的程度
        *   [perctl](http://help.scilab.org/docs/5.4.0/ja_JP/perctl.html) — 百分位数计算器
        *   [quart](http://help.scilab.org/docs/5.4.0/ja_JP/quart.html) — 第四个百分值计算器

        *   [Principal Component Analysis](http://help.scilab.org/docs/5.4.0/ja_JP/section_6adc5cd8f6753eb1d39b42b7135f4a9a.html)

            *   [pca](http://help.scilab.org/docs/5.4.0/ja_JP/pca.html) — 主成分分析法的归一化的变量
        *   [princomp](http://help.scilab.org/docs/5.4.0/ja_JP/princomp.html) — 主成分分析
        *   [show_pca](http://help.scilab.org/docs/5.4.0/ja_JP/show_pca.html) — 主成分分析的结果的可视化

        *   [Regression](http://help.scilab.org/docs/5.4.0/ja_JP/section_bcca82b50fbbc724d0888d7553893677.html)

            *   [regress](http://help.scilab.org/docs/5.4.0/ja_JP/regress.html) — 两个变量的回归系数

        *   [Sampling](http://help.scilab.org/docs/5.4.0/ja_JP/section_5ffca57e3edfd2d670e064e3437280e7.html)

            *   [sample](http://help.scilab.org/docs/5.4.0/ja_JP/sample.html) — 采样与更换
        *   [samplef](http://help.scilab.org/docs/5.4.0/ja_JP/samplef.html) — 从人口和它们的值替换的采样频率。
        *   [samwr](http://help.scilab.org/docs/5.4.0/ja_JP/samwr.html) — 无需更换取样

        *   [Summaries](http://help.scilab.org/docs/5.4.0/ja_JP/section_353d01a83a81f9716aaa2fa04e3a5799.html)

            *   [nfreq](http://help.scilab.org/docs/5.4.0/ja_JP/nfreq.html) — 频率的向量或矩阵中的值
        *   [tabul](http://help.scilab.org/docs/5.4.0/ja_JP/tabul.html) — 矩阵或向量值的频率

        *   [labostat](http://help.scilab.org/docs/5.4.0/ja_JP/labostat.html) — Scilab 统计工具箱

*   稀疏矩阵[Sparses Matrix](http://help.scilab.org/docs/5.4.0/ja_JP/section_b66fcac0bce62e0ff17afc7c4d8b5ae8.html)

    *   [Sparse Decompositions](http://help.scilab.org/docs/5.4.0/ja_JP/section_a3de94e0774e9b550da7620b3b4f0dca.html)

            *   [ludel](http://help.scilab.org/docs/5.4.0/ja_JP/ludel.html) — 与 lufact 一起使用的实用工具函数
        *   [lufact](http://help.scilab.org/docs/5.4.0/ja_JP/lufact.html) — 稀疏的 LU 分解
        *   [luget](http://help.scilab.org/docs/5.4.0/ja_JP/luget.html) — 稀疏的 LU 分解的发展
        *   [lusolve](http://help.scilab.org/docs/5.4.0/ja_JP/lusolve.html) — 一种稀疏线性系统解决方案
        *   [spchol](http://help.scilab.org/docs/5.4.0/ja_JP/spchol.html) — 稀疏乔莱斯基分解

        *   [Linear Equations (Iterative Solvers)](http://help.scilab.org/docs/5.4.0/ja_JP/section_4efea08ad5d4bec358298ecc9e95c12a.html)

            *   [gmres](http://help.scilab.org/docs/5.4.0/ja_JP/gmres.html) — 广义的最低残留方法
        *   [pcg](http://help.scilab.org/docs/5.4.0/ja_JP/pcg.html) — 共轭梯度法的 プリコンディショナ
        *   [qmr](http://help.scilab.org/docs/5.4.0/ja_JP/qmr.html) — プリコンディショナ 准最小剩余法

        *   [Sparse Matrix Manipulation](http://help.scilab.org/docs/5.4.0/ja_JP/section_cd730032ff0312a87294e02b97fc86e7.html)

            *   [issparse](http://help.scilab.org/docs/5.4.0/ja_JP/issparse.html) — 确定输入的值是否稀疏矩阵
        *   [nnz](http://help.scilab.org/docs/5.4.0/ja_JP/nnz.html) — 非零矩阵元素的数目
        *   [speye](http://help.scilab.org/docs/5.4.0/ja_JP/speye.html) — 稀疏矩阵
        *   [spones](http://help.scilab.org/docs/5.4.0/ja_JP/spones.html) — 稀疏矩阵
        *   [sprand](http://help.scilab.org/docs/5.4.0/ja_JP/sprand.html) — 随机稀疏矩阵
        *   [spzeros](http://help.scilab.org/docs/5.4.0/ja_JP/spzeros.html) — 稀疏零矩阵

        *   [Sparse Matrix Conversion](http://help.scilab.org/docs/5.4.0/ja_JP/section_81a82d3032c71d7d5c996e19bb7c1a7d.html)

            *   [adj2sp](http://help.scilab.org/docs/5.4.0/ja_JP/adj2sp.html) — 到邻接表单的稀疏矩阵。
        *   [full](http://help.scilab.org/docs/5.4.0/ja_JP/full.html) — 正常到一个稀疏矩阵的矩阵
        *   [mtlb_sparse](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_sparse.html) — 转换稀疏矩阵
        *   [sp2adj](http://help.scilab.org/docs/5.4.0/ja_JP/sp2adj.html) — 稀疏矩阵到邻接的表单
        *   [sparse](http://help.scilab.org/docs/5.4.0/ja_JP/sparse.html) — 定义稀疏矩阵
        *   [spcompack](http://help.scilab.org/docs/5.4.0/ja_JP/spcompack.html) — 转换压缩的邻接表示形式
        *   [spget](http://help.scilab.org/docs/5.4.0/ja_JP/spget.html) — 获取一个稀疏矩阵的条目

        *   [chfact](http://help.scilab.org/docs/5.4.0/ja_JP/chfact.html) — 稀疏乔莱斯基分解
    *   [chsolve](http://help.scilab.org/docs/5.4.0/ja_JP/chsolve.html) — 稀疏矩阵 コレスキーソルバ
    *   [ordmmd](http://help.scilab.org/docs/5.4.0/ja_JP/ordmmd.html) — 要计算的最低限度的三维数组规则

*   [UMFPACK Interface](http://help.scilab.org/docs/5.4.0/ja_JP/section_2e14a582ce124d7aa6aff2224c6e061f.html)

    *   [PlotSparse](http://help.scilab.org/docs/5.4.0/ja_JP/PlotSparse.html) — 绘制模式的非 nul 稀疏矩阵的元素
    *   [ReadHBSparse](http://help.scilab.org/docs/5.4.0/ja_JP/ReadHBSparse.html) — 读取哈维尔-波音稀疏格式文件
    *   [cond2sp](http://help.scilab.org/docs/5.4.0/ja_JP/cond2sp.html) — 计算的 2-范数的条件数 s.p.d.稀疏矩阵的近似
    *   [condestsp](http://help.scilab.org/docs/5.4.0/ja_JP/condestsp.html) — 估计一个稀疏矩阵的条件数
    *   [rafiter](http://help.scilab.org/docs/5.4.0/ja_JP/rafiter.html) — S p d...线性系统的迭代细化。 此函数已过时。
    *   [res_with_prec](http://help.scilab.org/docs/5.4.0/ja_JP/res_with_prec.html) — 计算残余的 r = Ax b 与精度
    *   [taucs_chdel](http://help.scilab.org/docs/5.4.0/ja_JP/taucs_chdel.html) — 效用函数与 taucs_chfact 一起使用
    *   [taucs_chfact](http://help.scilab.org/docs/5.4.0/ja_JP/taucs_chfact.html) — S.p.d.稀疏矩阵的乔 factorisation
    *   [taucs_chget](http://help.scilab.org/docs/5.4.0/ja_JP/taucs_chget.html) — 检索 scilab 级别的 ebe-pcg
    *   [taucs_chinfo](http://help.scilab.org/docs/5.4.0/ja_JP/taucs_chinfo.html) — 获取关于乔因素的资料
    *   [taucs_chsolve](http://help.scilab.org/docs/5.4.0/ja_JP/taucs_chsolve.html) — 解决线性稀疏 (s.p.d.） 系统鉴于乔因素
    *   [taucs_license](http://help.scilab.org/docs/5.4.0/ja_JP/taucs_license.html) — 显示的 taucs 许可证
    *   [umf_license](http://help.scilab.org/docs/5.4.0/ja_JP/umf_license.html) — 显示的 umfpack 许可证
    *   [umf_ludel](http://help.scilab.org/docs/5.4.0/ja_JP/umf_ludel.html) — 效用函数与 umf_lufact 一起使用
    *   [umf_lufact](http://help.scilab.org/docs/5.4.0/ja_JP/umf_lufact.html) — 稀疏矩阵的 Lu factorisation
    *   [umf_luget](http://help.scilab.org/docs/5.4.0/ja_JP/umf_luget.html) — 检索 lu scilab 一级的因素
    *   [umf_luinfo](http://help.scilab.org/docs/5.4.0/ja_JP/umf_luinfo.html) — 获取 LU 因素有关的信息
    *   [umf_lusolve](http://help.scilab.org/docs/5.4.0/ja_JP/umf_lusolve.html) — 解决由于 LU 因素线性稀疏系统
    *   [umfpack](http://help.scilab.org/docs/5.4.0/ja_JP/umfpack.html) — 解决稀疏线性系统

*   优化与仿真[Optimization and Simulation](http://help.scilab.org/docs/5.4.0/ja_JP/section_2d5a75a1199bc2cda3b42a2b96b2b424.html)

    *   [Semidefinite Programming](http://help.scilab.org/docs/5.4.0/ja_JP/section_2ba8a73e0a337425b0955862aea22d8a.html)

            *   [list2vec](http://help.scilab.org/docs/5.4.0/ja_JP/list2vec.html) — 串联到矩阵，列表条目。
        *   [lmisolver](http://help.scilab.org/docs/5.4.0/ja_JP/lmisolver.html) — LMI 规划求解
        *   [lmitool](http://help.scilab.org/docs/5.4.0/ja_JP/lmitool.html) — 要解决的 LMI 工具
        *   [aplat](http://help.scilab.org/docs/5.4.0/ja_JP/aplat.html) — 拼合的列表。
        *   [pack](http://help.scilab.org/docs/5.4.0/ja_JP/pack.html) — 压缩的块对角对称矩阵的列表。
        *   [recons](http://help.scilab.org/docs/5.4.0/ja_JP/recons.html) — Aplat 的逆函数。
        *   [semidef](http://help.scilab.org/docs/5.4.0/ja_JP/semidef.html) — 解决半正定的问题。
        *   [unpack](http://help.scilab.org/docs/5.4.0/ja_JP/unpack.html) — 解压缩块对角对称矩阵的列表。
        *   [vec2list](http://help.scilab.org/docs/5.4.0/ja_JP/vec2list.html) — List2vec 的逆函数。

        *   [Neldermead](http://help.scilab.org/docs/5.4.0/ja_JP/section_94806b6f99c310115e9b97a0a5a49a4d.html)

            *   [fminsearch](http://help.scilab.org/docs/5.4.0/ja_JP/fminsearch.html) — 计算无约束的 minimimum 给定函数与单纯米德算法。
        *   [neldermead](http://help.scilab.org/docs/5.4.0/ja_JP/neldermead.html) — 提供了直接搜索优化算法。
        *   [neldermead_overview](http://help.scilab.org/docs/5.4.0/ja_JP/neldermead_overview.html) — 内尔德米德工具箱的概览。
        *   [nmplot](http://help.scilab.org/docs/5.4.0/ja_JP/nmplot.html) — 提供了直接搜索优化算法。
        *   [optimget](http://help.scilab.org/docs/5.4.0/ja_JP/optimget.html) — 查询优化的数据结构。
        *   [optimplotfunccount](http://help.scilab.org/docs/5.4.0/ja_JP/optimplotfunccount.html) — 绘制函数的一种优化算法的评价数目
        *   [optimplotfval](http://help.scilab.org/docs/5.4.0/ja_JP/optimplotfval.html) — 绘制一种优化算法函数的值
        *   [optimplotx](http://help.scilab.org/docs/5.4.0/ja_JP/optimplotx.html) — 绘制的一种优化算法参数的值
        *   [optimset](http://help.scilab.org/docs/5.4.0/ja_JP/optimset.html) — 配置并返回一个优化的数据结构。

        *   [Optimization base](http://help.scilab.org/docs/5.4.0/ja_JP/section_cd670025d6df0059024ef896120bead7.html)

            *   [optimbase](http://help.scilab.org/docs/5.4.0/ja_JP/optimbase.html) — 为一般优化组件提供一个抽象类。

        *   [Optimization simplex](http://help.scilab.org/docs/5.4.0/ja_JP/section_39baca8b971e81981e1173d9888f113d.html)

            *   [optimsimplex](http://help.scilab.org/docs/5.4.0/ja_JP/optimsimplex.html) — 管理单纯与任意数量的点。

        *   [fsolve](http://help.scilab.org/docs/5.4.0/ja_JP/fsolve.html) —  求解非线性联立方程组f(x)=0的解
    *   [qp_solve](http://help.scilab.org/docs/5.4.0/ja_JP/qp_solve.html) — 内置线性第二按揭保险计划规划求解
    *   [qpsolve](http://help.scilab.org/docs/5.4.0/ja_JP/qpsolve.html) — 线性二次按揭保险计划规划求解
    *   [NDcost](http://help.scilab.org/docs/5.4.0/ja_JP/NDcost.html) — 一般外部羊毛计算渐变使用有限的差异
    *   [datafit](http://help.scilab.org/docs/5.4.0/ja_JP/datafit.html) — 基于测量数据的参数辨识
    *   [derivative](http://help.scilab.org/docs/5.4.0/ja_JP/derivative.html) — 函数的近似衍生品
    *   [fit_dat](http://help.scilab.org/docs/5.4.0/ja_JP/fit_dat.html) — 基于测量数据的参数辨识
    *   [karmarkar](http://help.scilab.org/docs/5.4.0/ja_JP/karmarkar.html) — 解决线性优化问题。
    *   [leastsq](http://help.scilab.org/docs/5.4.0/ja_JP/leastsq.html) — 求解非线性最小二乘问题
    *   [lsqrsolve](http://help.scilab.org/docs/5.4.0/ja_JP/lsqrsolve.html) — 尽量减少非线性函数，夸算法的平方和
    *   [optim](http://help.scilab.org/docs/5.4.0/ja_JP/optim.html) — 非线性优化例程
    *   [qld](http://help.scilab.org/docs/5.4.0/ja_JP/qld.html) — 线性二次编程规划求解
    *   [readmps](http://help.scilab.org/docs/5.4.0/ja_JP/readmps.html) — 从 MPS 文件中读取一个线性的程序。

*   遗传算法[Genetic Algorithms](http://help.scilab.org/docs/5.4.0/ja_JP/section_548e0b5cda775b7ce2bd4f800488fcc5.html)

    *   [Algorithms](http://help.scilab.org/docs/5.4.0/ja_JP/section_629e1750e2b90e5b183a123684b5db2a.html)

            *   [optim_ga](http://help.scilab.org/docs/5.4.0/ja_JP/optim_ga.html) — 一种灵活的遗传算法
        *   [optim_moga](http://help.scilab.org/docs/5.4.0/ja_JP/optim_moga.html) — 多目标遗传算法
        *   [optim_nsga](http://help.scilab.org/docs/5.4.0/ja_JP/optim_nsga.html) — 多目标 Niched 共享遗传算法
        *   [optim_nsga2](http://help.scilab.org/docs/5.4.0/ja_JP/optim_nsga2.html) — 多目标 Niched 共享遗传算法版本 2

        *   [Utilities](http://help.scilab.org/docs/5.4.0/ja_JP/section_c7c841cf4263f5cab6a07825e493543f.html)

            *   [coding_ga_binary](http://help.scilab.org/docs/5.4.0/ja_JP/coding_ga_binary.html) — 一个函数，执行二进制和连续表示形式之间的转换
        *   [coding_ga_identity](http://help.scilab.org/docs/5.4.0/ja_JP/coding_ga_identity.html) — "无操作"转换函数
        *   [crossover_ga_binary](http://help.scilab.org/docs/5.4.0/ja_JP/crossover_ga_binary.html) — 对于二进制代码的交叉功能
        *   [crossover_ga_default](http://help.scilab.org/docs/5.4.0/ja_JP/crossover_ga_default.html) — 连续变量的函数的交叉功能
        *   [init_ga_default](http://help.scilab.org/docs/5.4.0/ja_JP/init_ga_default.html) — 人口初始化函数
        *   [mutation_ga_binary](http://help.scilab.org/docs/5.4.0/ja_JP/mutation_ga_binary.html) — 一个函数，执行二进制突变
        *   [mutation_ga_default](http://help.scilab.org/docs/5.4.0/ja_JP/mutation_ga_default.html) — 连续变量突变功能
        *   [pareto_filter](http://help.scilab.org/docs/5.4.0/ja_JP/pareto_filter.html) — 一个函数，提取非主导从一组解决方案
        *   [selection_ga_elitist](http://help.scilab.org/docs/5.4.0/ja_JP/selection_ga_elitist.html) — '精英' 选择功能
        *   [selection_ga_random](http://help.scilab.org/docs/5.4.0/ja_JP/selection_ga_random.html) — 一个函数，执行随机选择的个人

*   [Simulated Annealing](http://help.scilab.org/docs/5.4.0/ja_JP/section_f3b2cd76d3c22da6b397d84bb2a78cbd.html)

    *   [Algorithms](http://help.scilab.org/docs/5.4.0/ja_JP/section_e2fac8837bf9967ec4655611826392f7.html)

            *   [optim_sa](http://help.scilab.org/docs/5.4.0/ja_JP/optim_sa.html) — 模拟退火优化方法

        *   [Utilities](http://help.scilab.org/docs/5.4.0/ja_JP/section_79cc77149d7769bd2c9b265478c73978.html)

            *   [accept_func_default](http://help.scilab.org/docs/5.4.0/ja_JP/accept_func_default.html) — 默认模拟退火词义函数。
        *   [accept_func_vfsa](http://help.scilab.org/docs/5.4.0/ja_JP/accept_func_vfsa.html) — 非常快速模拟退火的词义函数。
        *   [compute_initial_temp](http://help.scilab.org/docs/5.4.0/ja_JP/compute_initial_temp.html) — SA 功能允许来计算模拟退火的初始温度
        *   [neigh_func_csa](http://help.scilab.org/docs/5.4.0/ja_JP/neigh_func_csa.html) — 有关模拟退火的古典邻里关系
        *   [neigh_func_default](http://help.scilab.org/docs/5.4.0/ja_JP/neigh_func_default.html) — 一个 SA 函数计算给定的点的邻居
        *   [neigh_func_fsa](http://help.scilab.org/docs/5.4.0/ja_JP/neigh_func_fsa.html) — 快速模拟退火 neghborhood 关系
        *   [neigh_func_vfsa](http://help.scilab.org/docs/5.4.0/ja_JP/neigh_func_vfsa.html) — 非常快速模拟退火邻里关系
        *   [temp_law_csa](http://help.scilab.org/docs/5.4.0/ja_JP/temp_law_csa.html) — 古典温度下降法
        *   [temp_law_default](http://help.scilab.org/docs/5.4.0/ja_JP/temp_law_default.html) — 一个 SA 函数，计算温度的下一阶段的温度
        *   [temp_law_fsa](http://help.scilab.org/docs/5.4.0/ja_JP/temp_law_fsa.html) — 位和哈特利快速模拟退火算法
        *   [temp_law_huang](http://help.scilab.org/docs/5.4.0/ja_JP/temp_law_huang.html) — 黄温度降低为模拟退火法
        *   [temp_law_vfsa](http://help.scilab.org/docs/5.4.0/ja_JP/temp_law_vfsa.html) — 此函数可实现非常快速模拟退火从 L.贝尔

*   XML管理[XML Management](http://help.scilab.org/docs/5.4.0/ja_JP/section_89f2b94b29ed8f98a90dd6bedef97e13.html)

    *   [XMLObjects](http://help.scilab.org/docs/5.4.0/ja_JP/XMLObjects.html) — 若要描述的 XML 对象的不同属性
    *   [xmlAddNs](http://help.scilab.org/docs/5.4.0/ja_JP/xmlAddNs.html) — 添加到 XML 元素的命名空间
    *   [xmlAsNumber](http://help.scilab.org/docs/5.4.0/ja_JP/xmlAsNumber.html) — XPath 查询结果到的行中的数字
    *   [xmlAsText](http://help.scilab.org/docs/5.4.0/ja_JP/xmlAsText.html) — 成字符串线 XPath 查询结果
    *   [xmlDTD](http://help.scilab.org/docs/5.4.0/ja_JP/xmlDTD.html) — 创建 XML DTD 的对象
    *   [xmlDelete](http://help.scilab.org/docs/5.4.0/ja_JP/xmlDelete.html) — 移除 XML 文档
    *   [xmlDocument](http://help.scilab.org/docs/5.4.0/ja_JP/xmlDocument.html) — 创建新的 XML 文档
    *   [xmlDump](http://help.scilab.org/docs/5.4.0/ja_JP/xmlDump.html) — XML 对象转储
    *   [xmlElement](http://help.scilab.org/docs/5.4.0/ja_JP/xmlElement.html) — 若要创建新的 XML 元素
    *   [xmlFormat](http://help.scilab.org/docs/5.4.0/ja_JP/xmlFormat.html) — 若要设置格式的 XML Scilab 变量
    *   [xmlGetNsByHref](http://help.scilab.org/docs/5.4.0/ja_JP/xmlGetNsByHref.html) — 要获取其名称的 href
    *   [xmlGetNsByPrefix](http://help.scilab.org/docs/5.4.0/ja_JP/xmlGetNsByPrefix.html) — 获取命名空间前缀
    *   [xmlGetOpenDocs](http://help.scilab.org/docs/5.4.0/ja_JP/xmlGetOpenDocs.html) — 获取所有打开的 XML 文档或 XML 验证文件。
    *   [xmlIsValidObject](http://help.scilab.org/docs/5.4.0/ja_JP/xmlIsValidObject.html) — 确定 XML 对象存在
    *   [xmlNs](http://help.scilab.org/docs/5.4.0/ja_JP/xmlNs.html) — 若要创建新的 XML 命名空间
    *   [xmlRead](http://help.scilab.org/docs/5.4.0/ja_JP/xmlRead.html) — 从远程或本地加载 XML 流
    *   [xmlReadStr](http://help.scilab.org/docs/5.4.0/ja_JP/xmlReadStr.html) — 从字符串加载 XML 树
    *   [xmlRelaxNG](http://help.scilab.org/docs/5.4.0/ja_JP/xmlRelaxNG.html) — 创建 XML Relax NG 对象
    *   [xmlRemove](http://help.scilab.org/docs/5.4.0/ja_JP/xmlRemove.html) — 要移除的元素或元素的从父母
    *   [xmlSchema](http://help.scilab.org/docs/5.4.0/ja_JP/xmlSchema.html) — 若要创建 XML 架构对象
    *   [xmlSetAttributes](http://help.scilab.org/docs/5.4.0/ja_JP/xmlSetAttributes.html) — 若要设置的属性名称和值。
    *   [xmlValidate](http://help.scilab.org/docs/5.4.0/ja_JP/xmlValidate.html) — 通过 DTD、 Relax NG 或架构来验证文档。
    *   [xmlWrite](http://help.scilab.org/docs/5.4.0/ja_JP/xmlWrite.html) — 将 XML 文档写入到文件
    *   [xmlXPath](http://help.scilab.org/docs/5.4.0/ja_JP/xmlXPath.html) — XPath 查询来创建 XML 文档

*   文件输入输出函数[Files : Input/Output functions](http://help.scilab.org/docs/5.4.0/ja_JP/section_ce364d1fe248015591a43a41ac11aa86.html)

    *   [Directory](http://help.scilab.org/docs/5.4.0/ja_JP/section_fa39f6ac5d434b689b0555db55c46fb6.html)

            *   [chdir](http://help.scilab.org/docs/5.4.0/ja_JP/chdir.html) — 若要更改 Scilab 当前目录
        *   [createdir](http://help.scilab.org/docs/5.4.0/ja_JP/createdir.html) — 创建一个新目录
        *   [dir](http://help.scilab.org/docs/5.4.0/ja_JP/dir.html) — 要获取的文件列表
        *   [isdir](http://help.scilab.org/docs/5.4.0/ja_JP/isdir.html) — 参数确定的目录路径吗？
        *   [ls](http://help.scilab.org/docs/5.4.0/ja_JP/ls.html) — 查看文件
        *   [mkdir](http://help.scilab.org/docs/5.4.0/ja_JP/mkdir.html) — 新的目录
        *   [pwd](http://help.scilab.org/docs/5.4.0/ja_JP/pwd.html) — 获取 Scilab 当前目录
        *   [removedir](http://help.scilab.org/docs/5.4.0/ja_JP/removedir.html) — 删除目录
        *   [rmdir](http://help.scilab.org/docs/5.4.0/ja_JP/rmdir.html) — 删除目录

        *   [Paths - Filenames](http://help.scilab.org/docs/5.4.0/ja_JP/section_ef44803d7a79f385ef562efae1aa2c5b.html)

            *   [basename](http://help.scilab.org/docs/5.4.0/ja_JP/basename.html) — 除去目录和文件名的后缀
        *   [dirname](http://help.scilab.org/docs/5.4.0/ja_JP/dirname.html) — 获取目录中的文件的名称
        *   [fileext](http://help.scilab.org/docs/5.4.0/ja_JP/fileext.html) — 返回的文件路径的扩展名
        *   [fileparts](http://help.scilab.org/docs/5.4.0/ja_JP/fileparts.html) — 返回的路径的文件路径、 文件名和扩展名
        *   [filesep](http://help.scilab.org/docs/5.4.0/ja_JP/filesep.html) — 返回目录上当前平台 リセパレータ
        *   [fullfile](http://help.scilab.org/docs/5.4.0/ja_JP/fullfile.html) — 生成完整的文件名，从部件
        *   [fullpath](http://help.scilab.org/docs/5.4.0/ja_JP/fullpath.html) — 若要创建指定的相对路径名称的完整路径名称。
        *   [get_absolute_file_path](http://help.scilab.org/docs/5.4.0/ja_JP/get_absolute_file_path.html) — 打印在 Scilab 中打开的文件的完整路径名称。
        *   [getdrives](http://help.scilab.org/docs/5.4.0/ja_JP/getdrives.html) — 要获取所有的驱动器字母装入的文件系统的计算机。
        *   [getlongpathname](http://help.scilab.org/docs/5.4.0/ja_JP/getlongpathname.html) — 获取长路径名称 （仅 Windows）
        *   [getrelativefilename](http://help.scilab.org/docs/5.4.0/ja_JP/getrelativefilename.html) — 绝对的绝对文件名和目录，返回一个相对文件名称。
        *   [getshortpathname](http://help.scilab.org/docs/5.4.0/ja_JP/getshortpathname.html) — 获取短路径名称 （仅 Windows）
        *   [pathconvert](http://help.scilab.org/docs/5.4.0/ja_JP/pathconvert.html) — 转换 POSIX 和 windows 之间的路径名。
        *   [pathsep](http://help.scilab.org/docs/5.4.0/ja_JP/pathsep.html) — 返回当前平台 パスセパレータ
        *   [tempname](http://help.scilab.org/docs/5.4.0/ja_JP/tempname.html) — 临时文件的唯一名称

        *   [copyfile](http://help.scilab.org/docs/5.4.0/ja_JP/copyfile.html) — 将该文件复制
    *   [deletefile](http://help.scilab.org/docs/5.4.0/ja_JP/deletefile.html) — 要删除一个文件
    *   [dispfiles](http://help.scilab.org/docs/5.4.0/ja_JP/dispfiles.html) — 查看打开的文件的属性
    *   [fileinfo](http://help.scilab.org/docs/5.4.0/ja_JP/fileinfo.html) — 文件打印信息
    *   [findfiles](http://help.scilab.org/docs/5.4.0/ja_JP/findfiles.html) — 查找具有给定 filespec 中的所有文件
    *   [fprintf](http://help.scilab.org/docs/5.4.0/ja_JP/fprintf.html) — C 语言标准函数的仿真
    *   [fprintfMat](http://help.scilab.org/docs/5.4.0/ja_JP/fprintfMat.html) — 写入矩阵的文件...
    *   [fscanfMat](http://help.scilab.org/docs/5.4.0/ja_JP/fscanfMat.html) — 矩阵是从文本文件中读取的。
    *   [getmd5](http://help.scilab.org/docs/5.4.0/ja_JP/getmd5.html) — 获取 md5 校验和
    *   [io](http://help.scilab.org/docs/5.4.0/ja_JP/io.html) — 变量，返回的标准输入和标准输出 （文件描述符）。
    *   [isfile](http://help.scilab.org/docs/5.4.0/ja_JP/isfile.html) — 参数确定的文件吗？
    *   [listfiles](http://help.scilab.org/docs/5.4.0/ja_JP/listfiles.html) — 文件的列表
    *   [listvarinfile](http://help.scilab.org/docs/5.4.0/ja_JP/listvarinfile.html) — 获取您所保存的数据文件的内容的列表
    *   [maxfiles](http://help.scilab.org/docs/5.4.0/ja_JP/maxfiles.html) — 可以在同一时间 Scilab 打开的文件数最大值。
    *   [mclearerr](http://help.scilab.org/docs/5.4.0/ja_JP/mclearerr.html) — 重放 バイナリファイルアクセスエラー
    *   [mclose](http://help.scilab.org/docs/5.4.0/ja_JP/mclose.html) — 关闭打开的文件
    *   [mdelete](http://help.scilab.org/docs/5.4.0/ja_JP/mdelete.html) — 删除文件
    *   [meof](http://help.scilab.org/docs/5.4.0/ja_JP/meof.html) — 要确定是否已到达文件结尾
    *   [merror](http://help.scilab.org/docs/5.4.0/ja_JP/merror.html) — 找出关于文件访问错误指示灯
    *   [mfprintf](http://help.scilab.org/docs/5.4.0/ja_JP/mfprintf.html) — 转换、 设置格式和向文件中写入数据
    *   [mfscanf](http://help.scilab.org/docs/5.4.0/ja_JP/mfscanf.html) — 读取输入字符串 （接口的 C 语言 sscanf 函数） 从
    *   [mget](http://help.scilab.org/docs/5.4.0/ja_JP/mget.html) — 在二进制文件中的字节格式设置或读取该单词，转换为 int 数据类型
    *   [mgetl](http://help.scilab.org/docs/5.4.0/ja_JP/mgetl.html) — 从 ASCII 文件读取的行
    *   [mgetstr](http://help.scilab.org/docs/5.4.0/ja_JP/mgetstr.html) — 导入文本
    *   [mopen](http://help.scilab.org/docs/5.4.0/ja_JP/mopen.html) — 打开的文件
    *   [movefile](http://help.scilab.org/docs/5.4.0/ja_JP/movefile.html) — 要移动的文件或目录
    *   [mput](http://help.scilab.org/docs/5.4.0/ja_JP/mput.html) — 字节或二进制格式写一个字
    *   [mputl](http://help.scilab.org/docs/5.4.0/ja_JP/mputl.html) — 将一个字符串写入到 ASCII 文件
    *   [mputstr](http://help.scilab.org/docs/5.4.0/ja_JP/mputstr.html) — 将一个字符串写入到文件
    *   [mseek](http://help.scilab.org/docs/5.4.0/ja_JP/mseek.html) — 若要设置二进制文件中的当前位置。
    *   [mtell](http://help.scilab.org/docs/5.4.0/ja_JP/mtell.html) — 二进制文件管理
    *   [newest](http://help.scilab.org/docs/5.4.0/ja_JP/newest.html) — 返回一组文件中的最新文件
    *   [save_format](http://help.scilab.org/docs/5.4.0/ja_JP/save_format.html) — 使用"保存"创建的文件的格式
    *   [scanf](http://help.scilab.org/docs/5.4.0/ja_JP/scanf.html) — 转换格式 stdin 输入
    *   [scanf_conversion](http://help.scilab.org/docs/5.4.0/ja_JP/scanf_conversion.html) — scanf，sscanf，fscanf 转换说明符
    *   [sscanf](http://help.scilab.org/docs/5.4.0/ja_JP/sscanf.html) — 指定的字符串输入的格式转换

*   输入输出[Input/Output functions](http://help.scilab.org/docs/5.4.0/ja_JP/section_86533d65efa39a34003cf0668a2c7a09.html)

    *   [file](http://help.scilab.org/docs/5.4.0/ja_JP/file.html) — 文件管理
    *   [getenv](http://help.scilab.org/docs/5.4.0/ja_JP/getenv.html) — 获取环境变量的值
    *   [getio](http://help.scilab.org/docs/5.4.0/ja_JP/getio.html) — 获取 Scilab 输入/输出逻辑单元
    *   [getpid](http://help.scilab.org/docs/5.4.0/ja_JP/getpid.html) — 获得 Scilab 进程 ID
    *   [getscilabkeywords](http://help.scilab.org/docs/5.4.0/ja_JP/getscilabkeywords.html) — 返回所有 Scilab 关键字的列表。
    *   [halt](http://help.scilab.org/docs/5.4.0/ja_JP/halt.html) — 停止运行
    *   [host](http://help.scilab.org/docs/5.4.0/ja_JP/host.html) — 运行 Unix 或 DOS 命令
    *   [input](http://help.scilab.org/docs/5.4.0/ja_JP/input.html) — 提示用户输入
    *   [load](http://help.scilab.org/docs/5.4.0/ja_JP/load.html) — 您保存一个或多个变量
    *   [read](http://help.scilab.org/docs/5.4.0/ja_JP/read.html) — 加载矩阵
    *   [read4b](http://help.scilab.org/docs/5.4.0/ja_JP/read4b.html) — fortran ファイルバイナリ 负载
    *   [readb](http://help.scilab.org/docs/5.4.0/ja_JP/readb.html) — fortran ファイルバイナリ 负载
    *   [save](http://help.scilab.org/docs/5.4.0/ja_JP/save.html) — 二进制文件、 一个或多个变量
    *   [setenv](http://help.scilab.org/docs/5.4.0/ja_JP/setenv.html) — E 设置环境变量的值
    *   [unix](http://help.scilab.org/docs/5.4.0/ja_JP/unix.html) — 至外壳 (sh)
    *   [unix_g](http://help.scilab.org/docs/5.4.0/ja_JP/unix_g.html) — 到外壳程序 (sh)，重定向输出到一个变量
    *   [unix_s](http://help.scilab.org/docs/5.4.0/ja_JP/unix_s.html) — 无输出，运行 shell (sh) 命令
    *   [unix_w](http://help.scilab.org/docs/5.4.0/ja_JP/unix_w.html) — 到外壳程序 (sh)，以将输出重定向到一个 Scilab 窗口
    *   [unix_x](http://help.scilab.org/docs/5.4.0/ja_JP/unix_x.html) — 壳 (sh) 命令，将输出窗口中重定向
    *   [writb](http://help.scilab.org/docs/5.4.0/ja_JP/writb.html) — fortran 文件二进制文件写入
    *   [write](http://help.scilab.org/docs/5.4.0/ja_JP/write.html) — 写一个格式的文件
    *   [write4b](http://help.scilab.org/docs/5.4.0/ja_JP/write4b.html) — Fortran ファイルバイナリ 写道：

*   绘图[Graphics](http://help.scilab.org/docs/5.4.0/ja_JP/section_7bd1c72ce862b4c7a6656da70402650a.html)

    *   [2d_plot](http://help.scilab.org/docs/5.4.0/ja_JP/section_689e1e28906946c44c7b3073dcda3678.html)

            *   [LineSpec](http://help.scilab.org/docs/5.4.0/ja_JP/LineSpec.html) — 轻松地自定义规范的绘制线条的外观
        *   [Matplot](http://help.scilab.org/docs/5.4.0/ja_JP/Matplot.html) — 矩阵彩色 2D 地块
        *   [Matplot1](http://help.scilab.org/docs/5.4.0/ja_JP/Matplot1.html) — 矩阵的 2D 颜色出图
        *   [Matplot_properties](http://help.scilab.org/docs/5.4.0/ja_JP/Matplot_properties.html) — Matplot 实体属性的说明
        *   [Sfgrayplot](http://help.scilab.org/docs/5.4.0/ja_JP/Sfgrayplot.html) — 由函数定义的二维彩色绘图表面平滑
        *   [Sgrayplot](http://help.scilab.org/docs/5.4.0/ja_JP/Sgrayplot.html) — 彩色曲线的 2 维平滑阴谋
        *   [champ](http://help.scilab.org/docs/5.4.0/ja_JP/champ.html) — 2 维向量场阴谋
        *   [champ1](http://help.scilab.org/docs/5.4.0/ja_JP/champ1.html) — 绘制 2D 向量场带有彩色箭头
        *   [champ_properties](http://help.scilab.org/docs/5.4.0/ja_JP/champ_properties.html) — 2 维向量的字段的实体属性的描述
        *   [comet](http://help.scilab.org/docs/5.4.0/ja_JP/comet.html) — 2 维的彗星动画的地块。
        *   [contour2d](http://help.scilab.org/docs/5.4.0/ja_JP/contour2d.html) — 2D 绘图上绘制曲面
        *   [contour2di](http://help.scilab.org/docs/5.4.0/ja_JP/contour2di.html) — 计算的 2D 绘图的表面的轮廓
        *   [contourf](http://help.scilab.org/docs/5.4.0/ja_JP/contourf.html) — 绘制填充的轮廓表面上 2D 绘图
        *   [errbar](http://help.scilab.org/docs/5.4.0/ja_JP/errbar.html) — 在二维绘图中添加垂直误差线
        *   [fchamp](http://help.scilab.org/docs/5.4.0/ja_JP/fchamp.html) — 1F 2 三维场的常微分方程 (ODE)
        *   [fcontour2d](http://help.scilab.org/docs/5.4.0/ja_JP/fcontour2d.html) — 绘制一个二维绘图函数中定义的表面的轮廓
        *   [fec](http://help.scilab.org/docs/5.4.0/ja_JP/fec.html) — 在三角网格定义的函数的伪彩色出图
        *   [fec_properties](http://help.scilab.org/docs/5.4.0/ja_JP/fec_properties.html) — fec 实体属性的说明
        *   [fgrayplot](http://help.scilab.org/docs/5.4.0/ja_JP/fgrayplot.html) — 由函数定义的颜色 2D 绘图表面
        *   [fplot2d](http://help.scilab.org/docs/5.4.0/ja_JP/fplot2d.html) — 二维曲线定义函数绘图
        *   [grayplot](http://help.scilab.org/docs/5.4.0/ja_JP/grayplot.html) — 2 D 颜色表面地积
        *   [grayplot_properties](http://help.scilab.org/docs/5.4.0/ja_JP/grayplot_properties.html) — 实体 grayplot 属性的描述
        *   [graypolarplot](http://help.scilab.org/docs/5.4.0/ja_JP/graypolarplot.html) — 表面的极地的 2D 颜色出图
        *   [histplot](http://help.scilab.org/docs/5.4.0/ja_JP/histplot.html) — 若要绘制直方图
        *   [paramfplot2d](http://help.scilab.org/docs/5.4.0/ja_JP/paramfplot2d.html) — 2 D 动画曲线函数绘图中定义的
        *   [plot](http://help.scilab.org/docs/5.4.0/ja_JP/plot.html) — 2D 绘图
        *   [plot2d](http://help.scilab.org/docs/5.4.0/ja_JP/plot2d.html) — 2D 绘图
        *   [plot2d1](http://help.scilab.org/docs/5.4.0/ja_JP/plot2d1.html) — 2 维绘图 (对数轴) (已弃用)
        *   [plot2d2](http://help.scilab.org/docs/5.4.0/ja_JP/plot2d2.html) — 2 维绘图 （楼梯功能）
        *   [plot2d3](http://help.scilab.org/docs/5.4.0/ja_JP/plot2d3.html) — 2 维绘图 （垂直栏）
        *   [plot2d4](http://help.scilab.org/docs/5.4.0/ja_JP/plot2d4.html) — 2 维绘图 （箭头格式）
        *   [polarplot](http://help.scilab.org/docs/5.4.0/ja_JP/polarplot.html) — 极地的阴谋

        *   [3d_plot](http://help.scilab.org/docs/5.4.0/ja_JP/section_788ffa4499e096bd8ccb2f4e1160d6a5.html)

            *   [comet3d](http://help.scilab.org/docs/5.4.0/ja_JP/comet3d.html) — 彗星动画的三维图。
        *   [contour](http://help.scilab.org/docs/5.4.0/ja_JP/contour.html) — 绘制轮廓曲面
        *   [eval3d](http://help.scilab.org/docs/5.4.0/ja_JP/eval3d.html) — 在网格上的函数值
        *   [eval3dp](http://help.scilab.org/docs/5.4.0/ja_JP/eval3dp.html) — 计算三个三维曲面的小平面参数表示形式
        *   [fac3d](http://help.scilab.org/docs/5.4.0/ja_JP/fac3d.html) — 3D 表面图 (已弃用)
        *   [fcontour](http://help.scilab.org/docs/5.4.0/ja_JP/fcontour.html) — 在已删除此函数的函数定义一个曲面绘制轮廓线。
        *   [fplot3d](http://help.scilab.org/docs/5.4.0/ja_JP/fplot3d.html) — 由函数定义曲面的三维的阴谋
        *   [fplot3d1](http://help.scilab.org/docs/5.4.0/ja_JP/fplot3d1.html) — 二次曲面定义 3D 灰色的函数或颜色级别绘制
        *   [genfac3d](http://help.scilab.org/docs/5.4.0/ja_JP/genfac3d.html) — 计算的小平面曲面
        *   [geom3d](http://help.scilab.org/docs/5.4.0/ja_JP/geom3d.html) — 后三个从 3D 投影到 2D 三维绘图
        *   [hist3d](http://help.scilab.org/docs/5.4.0/ja_JP/hist3d.html) — 3 维直方图
        *   [mesh](http://help.scilab.org/docs/5.4.0/ja_JP/mesh.html) — 3D 网格阴谋
        *   [milk_drop](http://help.scilab.org/docs/5.4.0/ja_JP/milk_drop.html) — 牛奶放 3D 功能
        *   [nf3d](http://help.scilab.org/docs/5.4.0/ja_JP/nf3d.html) — 以下参数为矩形小的
        *   [param3d](http://help.scilab.org/docs/5.4.0/ja_JP/param3d.html) — 三个三维绘图的曲线参数表示
        *   [param3d1](http://help.scilab.org/docs/5.4.0/ja_JP/param3d1.html) — 三个三维绘图的曲线参数表示
        *   [param3d_properties](http://help.scilab.org/docs/5.4.0/ja_JP/param3d_properties.html) — 三维曲线实体属性的说明
        *   [plot3d](http://help.scilab.org/docs/5.4.0/ja_JP/plot3d.html) — 三维曲面图
        *   [plot3d1](http://help.scilab.org/docs/5.4.0/ja_JP/plot3d1.html) — 弧形 3D 黑白或彩色绘图
        *   [plot3d2](http://help.scilab.org/docs/5.4.0/ja_JP/plot3d2.html) — 绘制由矩形的小平面定义的表面
        *   [plot3d3](http://help.scilab.org/docs/5.4.0/ja_JP/plot3d3.html) — 网由矩形的小平面定义的绘图面
        *   [secto3d](http://help.scilab.org/docs/5.4.0/ja_JP/secto3d.html) — 3 维曲面转换
        *   [surf](http://help.scilab.org/docs/5.4.0/ja_JP/surf.html) — 3D 表面图
        *   [surface_properties](http://help.scilab.org/docs/5.4.0/ja_JP/surface_properties.html) — 3D 实体属性的说明

        *   [annotation](http://help.scilab.org/docs/5.4.0/ja_JP/section_8085169d808395fa64d3da162a5a75f2.html)

            *   [captions](http://help.scilab.org/docs/5.4.0/ja_JP/captions.html) — 绘制图表标题
        *   [label_properties](http://help.scilab.org/docs/5.4.0/ja_JP/label_properties.html) — 标签实体属性的说明
        *   [legend](http://help.scilab.org/docs/5.4.0/ja_JP/legend.html) — 若要绘制图表的图例
        *   [legend_properties](http://help.scilab.org/docs/5.4.0/ja_JP/legend_properties.html) — 图例的实体属性的说明。
        *   [legends](http://help.scilab.org/docs/5.4.0/ja_JP/legends.html) — 绘制图表的图例
        *   [title](http://help.scilab.org/docs/5.4.0/ja_JP/title.html) — 显示图形窗口的标题
        *   [xlabel](http://help.scilab.org/docs/5.4.0/ja_JP/xlabel.html) — z 轴标签附加到
        *   [xtitle](http://help.scilab.org/docs/5.4.0/ja_JP/xtitle.html) — グラフィックスウ 印度向添加标题

        *   [axes_operations](http://help.scilab.org/docs/5.4.0/ja_JP/section_0abe187def8e2a3b415b20dd1e595a4c.html)

            *   [axes_properties](http://help.scilab.org/docs/5.4.0/ja_JP/axes_properties.html) — 轴实体属性的说明
        *   [gca](http://help.scilab.org/docs/5.4.0/ja_JP/gca.html) — 返回当前坐标轴的句柄。
        *   [gda](http://help.scilab.org/docs/5.4.0/ja_JP/gda.html) — 获取默认轴 (轴) 的句柄。
        *   [graduate](http://help.scilab.org/docs/5.4.0/ja_JP/graduate.html) — 漂亮轴渐变
        *   [isoview](http://help.scilab.org/docs/5.4.0/ja_JP/isoview.html) — 等轴地积比例 （不更改窗口大小）
        *   [newaxes](http://help.scilab.org/docs/5.4.0/ja_JP/newaxes.html) — 创建一个新的轴实体
        *   [plotframe](http://help.scilab.org/docs/5.4.0/ja_JP/plotframe.html) — 网格并将其缩放到帧的情节...... 此函数已弃用。
        *   [replot](http://help.scilab.org/docs/5.4.0/ja_JP/replot.html) — 在当前窗口的图形重新绘制新的边界。
        *   [rotate_axes](http://help.scilab.org/docs/5.4.0/ja_JP/rotate_axes.html) — 以交互方式旋转坐标轴的句柄。
        *   [sca](http://help.scilab.org/docs/5.4.0/ja_JP/sca.html) — 若要设置当前轴实体
        *   [sda](http://help.scilab.org/docs/5.4.0/ja_JP/sda.html) — 设置默认的轴 （轴）。
        *   [subplot](http://help.scilab.org/docs/5.4.0/ja_JP/subplot.html) — 矩阵的子窗口的图形窗口
        *   [unzoom](http://help.scilab.org/docs/5.4.0/ja_JP/unzoom.html) — 要解锁图形缩放
        *   [zoom_rect](http://help.scilab.org/docs/5.4.0/ja_JP/zoom_rect.html) — 缩放到当前图形图的所选部分

        *   [axis](http://help.scilab.org/docs/5.4.0/ja_JP/section_745bd5815af95565d5928eb232d390fb.html)

            *   [axis_properties](http://help.scilab.org/docs/5.4.0/ja_JP/axis_properties.html) — 轴实体属性的说明
        *   [drawaxis](http://help.scilab.org/docs/5.4.0/ja_JP/drawaxis.html) — 绘制轴

        *   [bar_histogram](http://help.scilab.org/docs/5.4.0/ja_JP/section_e8cc1a0d71002759cd202e3c7cc38c01.html)

            *   [bar](http://help.scilab.org/docs/5.4.0/ja_JP/bar.html) — 直方图条
        *   [barh](http://help.scilab.org/docs/5.4.0/ja_JP/barh.html) — 直方图水平栏
        *   [barhomogenize](http://help.scilab.org/docs/5.4.0/ja_JP/barhomogenize.html) — 质化载当前坐标轴的图表

        *   [Color management](http://help.scilab.org/docs/5.4.0/ja_JP/section_a57289672b46e1bc02f960090b0cea88.html)

            *   [addcolor](http://help.scilab.org/docs/5.4.0/ja_JP/addcolor.html) — 若要将新的颜色添加到当前的颜色映射
        *   [autumncolormap](http://help.scilab.org/docs/5.4.0/ja_JP/autumncolormap.html) — 通过向红颜色映射中黄橙
        *   [bonecolormap](http://help.scilab.org/docs/5.4.0/ja_JP/bonecolormap.html) — 浅蓝色灰色地图
        *   [color](http://help.scilab.org/docs/5.4.0/ja_JP/color.html) — 获取颜色颜色 ID
        *   [color_list](http://help.scilab.org/docs/5.4.0/ja_JP/color_list.html) — 颜色名称的列表
        *   [colorbar](http://help.scilab.org/docs/5.4.0/ja_JP/colorbar.html) — 绘制条形图
        *   [colordef](http://help.scilab.org/docs/5.4.0/ja_JP/colordef.html) — 若要设置默认为显示不同的颜色配色方案
        *   [colormap](http://help.scilab.org/docs/5.4.0/ja_JP/colormap.html) — 定义颜色映射
        *   [coolcolormap](http://help.scilab.org/docs/5.4.0/ja_JP/coolcolormap.html) — 从青色到洋红色的颜色映射
        *   [coppercolormap](http://help.scilab.org/docs/5.4.0/ja_JP/coppercolormap.html) — 从黑色到明亮的铜色地图
        *   [getcolor](http://help.scilab.org/docs/5.4.0/ja_JP/getcolor.html) — 打开一个对话框，指示当前的颜色映射的颜色
        *   [graycolormap](http://help.scilab.org/docs/5.4.0/ja_JP/graycolormap.html) — 线性灰度颜色映射
        *   [hotcolormap](http://help.scilab.org/docs/5.4.0/ja_JP/hotcolormap.html) — 从红色到黄色颜色映射
        *   [hsv2rgb](http://help.scilab.org/docs/5.4.0/ja_JP/hsv2rgb.html) — 若要将 HSV 颜色转换为 RGB
        *   [hsvcolormap](http://help.scilab.org/docs/5.4.0/ja_JP/hsvcolormap.html) — 颜色色调-饱和度-值映射
        *   [jetcolormap](http://help.scilab.org/docs/5.4.0/ja_JP/jetcolormap.html) — 它是从蓝色到红色颜色映射
        *   [name2rgb](http://help.scilab.org/docs/5.4.0/ja_JP/name2rgb.html) — 返回的 RGB 值与指定的名称
        *   [oceancolormap](http://help.scilab.org/docs/5.4.0/ja_JP/oceancolormap.html) — 线性蓝颜色映射
        *   [pinkcolormap](http://help.scilab.org/docs/5.4.0/ja_JP/pinkcolormap.html) — 棕褐色调着色处理的黑白图像
        *   [rainbowcolormap](http://help.scilab.org/docs/5.4.0/ja_JP/rainbowcolormap.html) — 通过橙、 黄色、 绿色和蓝色从紫色到红色颜色映射
        *   [rgb2name](http://help.scilab.org/docs/5.4.0/ja_JP/rgb2name.html) — 返回颜色的名称
        *   [springcolormap](http://help.scilab.org/docs/5.4.0/ja_JP/springcolormap.html) — 它是从洋红黄色的颜色映射到
        *   [summercolormap](http://help.scilab.org/docs/5.4.0/ja_JP/summercolormap.html) — 从绿色，黄色的颜色映射到
        *   [whitecolormap](http://help.scilab.org/docs/5.4.0/ja_JP/whitecolormap.html) — 是完全白颜色映射
        *   [wintercolormap](http://help.scilab.org/docs/5.4.0/ja_JP/wintercolormap.html) — 从蓝到绿颜色映射

        *   [Datatips](http://help.scilab.org/docs/5.4.0/ja_JP/section_9fc288dd33dd298b9e35302efb6c47b9.html)

            *   [datatipCreate](http://help.scilab.org/docs/5.4.0/ja_JP/datatipCreate.html) — 以编程方式创建折线数据信息
        *   [datatipGetEntities](http://help.scilab.org/docs/5.4.0/ja_JP/datatipGetEntities.html) — 获取数据提示指定轴中的所有实体与兼容。
        *   [datatipGetStruct](http://help.scilab.org/docs/5.4.0/ja_JP/datatipGetStruct.html) — 部署数据提示从曲线或曲面的实体的数据结构。
        *   [datatipInitStruct](http://help.scilab.org/docs/5.4.0/ja_JP/datatipInitStruct.html) — 若要初始化的数据提示结构上指定的折线。
        *   [datatipsRemoveAll](http://help.scilab.org/docs/5.4.0/ja_JP/datatipsRemoveAll.html) — 若要删除所有数据提示折线上的集...
        *   [datatipManagerMode](http://help.scilab.org/docs/5.4.0/ja_JP/datatipManagerMode.html) — 切换或设置数据提示模式。
        *   [datatipMove](http://help.scilab.org/docs/5.4.0/ja_JP/datatipMove.html) — 移动指定的鼠标数据提示。
        *   [datatipRedraw](http://help.scilab.org/docs/5.4.0/ja_JP/datatipRedraw.html) — 以调整后的 3D 旋转，datatp 文本框中的位置
        *   [datatipRemove](http://help.scilab.org/docs/5.4.0/ja_JP/datatipRemove.html) — 若要删除所选数据提示
        *   [datatipRemoveAll](http://help.scilab.org/docs/5.4.0/ja_JP/datatipRemoveAll.html) — 若要删除所有数据提示一套的折线。
        *   [datatipSetDisplay](http://help.scilab.org/docs/5.4.0/ja_JP/datatipSetDisplay.html) — 探索的指定的点最近的数据提示。
        *   [datatipSetInterp](http://help.scilab.org/docs/5.4.0/ja_JP/datatipSetInterp.html) — 提示设置模式的位置之间的插值。
        *   [datatipSetOrientation](http://help.scilab.org/docs/5.4.0/ja_JP/datatipSetOrientation.html) — 查找数据提示指定点最接近。
        *   [datatipSetStruct](http://help.scilab.org/docs/5.4.0/ja_JP/datatipSetStruct.html) — 数据提示数据结构来保存曲线或曲面的实体。
        *   [datatipSetStyle](http://help.scilab.org/docs/5.4.0/ja_JP/datatipSetStyle.html) — 设置的指定的折线 データティップ 提示窗体。
        *   [datatipToggle](http://help.scilab.org/docs/5.4.0/ja_JP/datatipToggle.html) — 切换到数据模式提示。
        *   [datatips](http://help.scilab.org/docs/5.4.0/ja_JP/datatips.html) — 用于编辑工具，信息 (tips) 在曲线上的绘制。
        *   [orthProj](http://help.scilab.org/docs/5.4.0/ja_JP/orthProj.html) — 若要计算到折线的平面点上的正交投影

        *   [figure_operations](http://help.scilab.org/docs/5.4.0/ja_JP/section_52068a7a00a565ca7cdb6b6b0e3614cf.html)

            *   [clf](http://help.scilab.org/docs/5.4.0/ja_JP/clf.html) — 清除当前的数字，并将重置为默认值
        *   [drawlater](http://help.scilab.org/docs/5.4.0/ja_JP/drawlater.html) — 看不到子轴。
        *   [drawnow](http://help.scilab.org/docs/5.4.0/ja_JP/drawnow.html) — 绘制隐藏的图形实体。
        *   [figure_properties](http://help.scilab.org/docs/5.4.0/ja_JP/figure_properties.html) — 图形实体属性的说明
        *   [gcf](http://help.scilab.org/docs/5.4.0/ja_JP/gcf.html) — カレントグラフィックウインドウ 句柄年度回报。
        *   [gdf](http://help.scilab.org/docs/5.4.0/ja_JP/gdf.html) — 获取默认关系图 （图） 的句柄。
        *   [scf](http://help.scilab.org/docs/5.4.0/ja_JP/scf.html) — 若要指定当前图 (窗口)
        *   [sdf](http://help.scilab.org/docs/5.4.0/ja_JP/sdf.html) — 设置默认关系图 （图）。

        *   [geometric_shapes](http://help.scilab.org/docs/5.4.0/ja_JP/section_aa8d5f761bdc8294539cf4aaf7e1f308.html)

            *   [arc_properties](http://help.scilab.org/docs/5.4.0/ja_JP/arc_properties.html) — 弧 （ARC） 实体属性的说明
        *   [rectangle_properties](http://help.scilab.org/docs/5.4.0/ja_JP/rectangle_properties.html) — 矩形实体属性的说明
        *   [xarc](http://help.scilab.org/docs/5.4.0/ja_JP/xarc.html) — 若要绘制一个椭圆的一部分
        *   [xarcs](http://help.scilab.org/docs/5.4.0/ja_JP/xarcs.html) — 若要绘制椭圆集的一部分
        *   [xarrows](http://help.scilab.org/docs/5.4.0/ja_JP/xarrows.html) — 绘制一组的箭头
        *   [xfarc](http://help.scilab.org/docs/5.4.0/ja_JP/xfarc.html) — 填充的椭圆的一部分
        *   [xfarcs](http://help.scilab.org/docs/5.4.0/ja_JP/xfarcs.html) — 填充椭圆集的一部分
        *   [xfrect](http://help.scilab.org/docs/5.4.0/ja_JP/xfrect.html) — 使用填充矩形
        *   [xrect](http://help.scilab.org/docs/5.4.0/ja_JP/xrect.html) — 若要绘制一个矩形
        *   [xrects](http://help.scilab.org/docs/5.4.0/ja_JP/xrects.html) — 绘制矩形或填充一系列

        *   [handle](http://help.scilab.org/docs/5.4.0/ja_JP/section_a242798df615310ce61325cc81c7226c.html)

            *   [copy](http://help.scilab.org/docs/5.4.0/ja_JP/copy.html) — 复制的图形的实体。
        *   [delete](http://help.scilab.org/docs/5.4.0/ja_JP/delete.html) — 删除图形实体及其子级。
        *   [draw](http://help.scilab.org/docs/5.4.0/ja_JP/draw.html) — 绘图实体。
        *   [gce](http://help.scilab.org/docs/5.4.0/ja_JP/gce.html) — 获取当前实体的句柄。
        *   [ged](http://help.scilab.org/docs/5.4.0/ja_JP/ged.html) — Scilab 图形编辑器
        *   [get_figure_handle](http://help.scilab.org/docs/5.4.0/ja_JP/get_figure_handle.html) — 获取指定的图表的句柄的 ID
        *   [glue](http://help.scilab.org/docs/5.4.0/ja_JP/glue.html) — 加入一系列的图形实体的化合物。
        *   [is_handle_valid](http://help.scilab.org/docs/5.4.0/ja_JP/is_handle_valid.html) — 看到一组图形句柄是有效的。
        *   [relocate_handle](http://help.scilab.org/docs/5.4.0/ja_JP/relocate_handle.html) — 移动到层次结构图形的句柄。
        *   [swap_handles](http://help.scilab.org/docs/5.4.0/ja_JP/swap_handles.html) — 要替换图形分层两个句柄。
        *   [unglue](http://help.scilab.org/docs/5.4.0/ja_JP/unglue.html) — 受约束，以取代个别儿童的对象。

        *   [interaction](http://help.scilab.org/docs/5.4.0/ja_JP/section_654ebdcd61ef9210fa751874ce22e21c.html)

            *   [dragrect](http://help.scilab.org/docs/5.4.0/ja_JP/dragrect.html) — 用鼠标拖动矩形
        *   [edit_curv](http://help.scilab.org/docs/5.4.0/ja_JP/edit_curv.html) — 向图形曲线编辑器界面
        *   [eventhandlerfunctions](http://help.scilab.org/docs/5.4.0/ja_JP/eventhandlerfunctions.html) — 函数的原型可以用作事件处理程序。
        *   [locate](http://help.scilab.org/docs/5.4.0/ja_JP/locate.html) — 若要选择多个点的鼠标
        *   [seteventhandler](http://help.scilab.org/docs/5.4.0/ja_JP/seteventhandler.html) — 设置当前的事件句柄的图形窗格
        *   [xclick](http://help.scilab.org/docs/5.4.0/ja_JP/xclick.html) — 等待鼠标单击。
        *   [xgetmouse](http://help.scilab.org/docs/5.4.0/ja_JP/xgetmouse.html) — 获取鼠标的事件和当前的位置

        *   [load_save](http://help.scilab.org/docs/5.4.0/ja_JP/section_f4e9dea7a451420f203c0a817ce9914c.html)

            *   [xload](http://help.scilab.org/docs/5.4.0/ja_JP/xload.html) — 若要加载保存的图形
        *   [xsave](http://help.scilab.org/docs/5.4.0/ja_JP/xsave.html) — 若要保存的图形文件

        *   [pie](http://help.scilab.org/docs/5.4.0/ja_JP/section_439a576ddc54e0b7349a1c719933fb5c.html)

            *   [pie](http://help.scilab.org/docs/5.4.0/ja_JP/pie.html) — 绘制饼图

        *   [polygon](http://help.scilab.org/docs/5.4.0/ja_JP/section_96dab3a58e334dd7bd8c405fa380a4bd.html)

            *   [polyline_properties](http://help.scilab.org/docs/5.4.0/ja_JP/polyline_properties.html) — 折线实体属性的说明
        *   [xfpoly](http://help.scilab.org/docs/5.4.0/ja_JP/xfpoly.html) — 填充多边形
        *   [xfpolys](http://help.scilab.org/docs/5.4.0/ja_JP/xfpolys.html) — 填充一组多边形
        *   [xpoly](http://help.scilab.org/docs/5.4.0/ja_JP/xpoly.html) — 要绘制折线或多边形
        *   [xpolys](http://help.scilab.org/docs/5.4.0/ja_JP/xpolys.html) — 在一系列绘制多边形或折线
        *   [xrpoly](http://help.scilab.org/docs/5.4.0/ja_JP/xrpoly.html) — 绘制多边形

        *   [property](http://help.scilab.org/docs/5.4.0/ja_JP/section_b3e00948370e8fe45ad20f0fdb716031.html)

            *   [get](http://help.scilab.org/docs/5.4.0/ja_JP/get.html) — 若要获取从图形实体或用户界面对象的属性值。
        *   [set](http://help.scilab.org/docs/5.4.0/ja_JP/set.html) — 设置属性或用户界面对象或图形实体对象的值。

        *   [style](http://help.scilab.org/docs/5.4.0/ja_JP/section_38f2db549e13fd0b0e1eb97a8c49f157.html)

            *   [getlinestyle](http://help.scilab.org/docs/5.4.0/ja_JP/getlinestyle.html) — 选择线条样式。 该函数被废除。
        *   [getmark](http://help.scilab.org/docs/5.4.0/ja_JP/getmark.html) — 对话框中选择的标记符号。 过时的函数
        *   [getsymbol](http://help.scilab.org/docs/5.4.0/ja_JP/getsymbol.html) — 对话框中选择符号和其大小......过时的函数

        *   [text](http://help.scilab.org/docs/5.4.0/ja_JP/section_13d1d87830ada6328c4732c39e7813d7.html)

            *   [getfont](http://help.scilab.org/docs/5.4.0/ja_JP/getfont.html) — 字体选择对话框......，废除了函数。
        *   [graphics_fonts](http://help.scilab.org/docs/5.4.0/ja_JP/graphics_fonts.html) — 在图示描述中使用的字体
        *   [math_rendering_features_in_graphic](http://help.scilab.org/docs/5.4.0/ja_JP/math_rendering_features_in_graphic.html) — 在乳胶或 MathML 的语言中显示公式 Scilab 图形。
        *   [stringbox](http://help.scilab.org/docs/5.4.0/ja_JP/stringbox.html) — 计算的边界框的文本或标签
        *   [text_properties](http://help.scilab.org/docs/5.4.0/ja_JP/text_properties.html) — 文本实体属性的说明
        *   [titlepage](http://help.scilab.org/docs/5.4.0/ja_JP/titlepage.html) — 为中心的图形窗口中添加标题
        *   [xinfo](http://help.scilab.org/docs/5.4.0/ja_JP/xinfo.html) — 要绘制的字符串 メッセージサブウインドウ
        *   [xlfont](http://help.scilab.org/docs/5.4.0/ja_JP/xlfont.html) — 要查找加载字体加载图形上下文
        *   [xstring](http://help.scilab.org/docs/5.4.0/ja_JP/xstring.html) — 绘制字符串
        *   [xstringb](http://help.scilab.org/docs/5.4.0/ja_JP/xstringb.html) — 在框中绘制字符串
        *   [xstringl](http://help.scilab.org/docs/5.4.0/ja_JP/xstringl.html) — 计算，文本周围的框

        *   [transform](http://help.scilab.org/docs/5.4.0/ja_JP/section_65c7a27282e7efa063fc88498ee944c7.html)

            *   [move](http://help.scilab.org/docs/5.4.0/ja_JP/move.html) — 若要转换，移动图形实体和其儿童
        *   [rotate](http://help.scilab.org/docs/5.4.0/ja_JP/rotate.html) — 旋转点集的
        *   [scaling](http://help.scilab.org/docs/5.4.0/ja_JP/scaling.html) — 仿射变换的点集的

        *   [window_control](http://help.scilab.org/docs/5.4.0/ja_JP/section_1cc177aa60df483a2cde2f6d5447a489.html)

            *   [havewindow](http://help.scilab.org/docs/5.4.0/ja_JP/havewindow.html) — 返回 Scilab 窗口模式
        *   [show_window](http://help.scilab.org/docs/5.4.0/ja_JP/show_window.html) — 某些图形窗格中向前移动
        *   [winsid](http://help.scilab.org/docs/5.4.0/ja_JP/winsid.html) — 返回图形窗口的列表
        *   [xselect](http://help.scilab.org/docs/5.4.0/ja_JP/xselect.html) — 将当前窗口的图形移到前面

        *   [GlobalProperty](http://help.scilab.org/docs/5.4.0/ja_JP/GlobalProperty.html) — 它的情节或冲浪命令对象 （曲线、 曲面......)自定义的外观。
    *   [Graphics](http://help.scilab.org/docs/5.4.0/ja_JP/Graphics.html) — 图形库概述
    *   [alufunctions](http://help.scilab.org/docs/5.4.0/ja_JP/alufunctions.html) — 像素绘图函数
    *   [clear_pixmap](http://help.scilab.org/docs/5.4.0/ja_JP/clear_pixmap.html) — 要擦除位图缓冲区
    *   [Compound_properties](http://help.scilab.org/docs/5.4.0/ja_JP/Compound_properties.html) — 复合实体属性的说明
    *   [graphics_entities](http://help.scilab.org/docs/5.4.0/ja_JP/graphics_entities.html) — 图形实体的数据结构的描述
    *   [object_editor](http://help.scilab.org/docs/5.4.0/ja_JP/object_editor.html) — 图形对象编辑器功能的说明
    *   [pixel_drawing_mode](http://help.scilab.org/docs/5.4.0/ja_JP/pixel_drawing_mode.html) — 呈现的像素的位函数。
    *   [plzr](http://help.scilab.org/docs/5.4.0/ja_JP/plzr.html) — 杆 / 零阴谋
    *   [rubberbox](http://help.scilab.org/docs/5.4.0/ja_JP/rubberbox.html) — 矩形橡胶带框
    *   [segs_properties](http://help.scilab.org/docs/5.4.0/ja_JP/segs_properties.html) — 线段实体属性的说明
    *   [show_pixmap](http://help.scilab.org/docs/5.4.0/ja_JP/show_pixmap.html) — 若要在屏幕上发送位图缓冲区
    *   [square](http://help.scilab.org/docs/5.4.0/ja_JP/square.html) — 如集轴绘图比例 （更改窗口的大小）
    *   [twinkle](http://help.scilab.org/docs/5.4.0/ja_JP/twinkle.html) — Flash 图形实体
    *   [xbasr](http://help.scilab.org/docs/5.4.0/ja_JP/xbasr.html) — 重绘图形窗口
    *   [xchange](http://help.scilab.org/docs/5.4.0/ja_JP/xchange.html) — 成像素坐标的真实坐标
    *   [xclear](http://help.scilab.org/docs/5.4.0/ja_JP/xclear.html) — 清除图形窗口
    *   [xdel](http://help.scilab.org/docs/5.4.0/ja_JP/xdel.html) — 若要删除一个图形窗口
    *   [xget](http://help.scilab.org/docs/5.4.0/ja_JP/xget.html) — 获取图形上下文的当前值。 此函数已弃用。
    *   [xgetech](http://help.scilab.org/docs/5.4.0/ja_JP/xgetech.html) — 获取当前图形比例
    *   [xgraduate](http://help.scilab.org/docs/5.4.0/ja_JP/xgraduate.html) — 渐变轴
    *   [xgrid](http://help.scilab.org/docs/5.4.0/ja_JP/xgrid.html) — 将网格添加到 2D 绘图
    *   [xname](http://help.scilab.org/docs/5.4.0/ja_JP/xname.html) — 要更改当前窗口的图形的名称
    *   [xnumb](http://help.scilab.org/docs/5.4.0/ja_JP/xnumb.html) — 绘制数字
    *   [xpause](http://help.scilab.org/docs/5.4.0/ja_JP/xpause.html) — 暂停 Scilab
    *   [xsegs](http://help.scilab.org/docs/5.4.0/ja_JP/xsegs.html) — 绘制直线段未连接
    *   [xset](http://help.scilab.org/docs/5.4.0/ja_JP/xset.html) — 设置图形上下文的值。 此函数是受废除。
    *   [xsetech](http://help.scilab.org/docs/5.4.0/ja_JP/xsetech.html) — 情节： 设置 グラフィックウ 印度子窗口
    *   [xsetm](http://help.scilab.org/docs/5.4.0/ja_JP/xsetm.html) — 对话框来设置图形上下文的值。 旧的函数。

*   绘图：导出和打印[Graphics : exporting and printing](http://help.scilab.org/docs/5.4.0/ja_JP/section_eb0241ade4c0113bbed15b9f0393c14d.html)

    *   [driver](http://help.scilab.org/docs/5.4.0/ja_JP/driver.html) — 若要选择一个图形驱动程序
    *   [xend](http://help.scilab.org/docs/5.4.0/ja_JP/xend.html) — 关闭图形会话
    *   [xinit](http://help.scilab.org/docs/5.4.0/ja_JP/xinit.html) — 初始化图形驱动程序。
    *   [xs2bmp](http://help.scilab.org/docs/5.4.0/ja_JP/xs2bmp.html) — BMP 文件的输出图形。
    *   [xs2emf](http://help.scilab.org/docs/5.4.0/ja_JP/xs2emf.html) — （仅限 Windows） 输出到 EMF 文件的图形。
    *   [xs2eps](http://help.scilab.org/docs/5.4.0/ja_JP/xs2eps.html) — 为 EPS 文件的输出图形。
    *   [xs2gif](http://help.scilab.org/docs/5.4.0/ja_JP/xs2gif.html) — GIF 文件的输出图形。
    *   [xs2jpg](http://help.scilab.org/docs/5.4.0/ja_JP/xs2jpg.html) — Jpg 输出图形。
    *   [xs2pdf](http://help.scilab.org/docs/5.4.0/ja_JP/xs2pdf.html) — 将图形保存到一个 PDF 文件。
    *   [xs2png](http://help.scilab.org/docs/5.4.0/ja_JP/xs2png.html) — 输出到 PNG 文件的图形。
    *   [xs2ppm](http://help.scilab.org/docs/5.4.0/ja_JP/xs2ppm.html) — PPM 文件输出图形。
    *   [xs2ps](http://help.scilab.org/docs/5.4.0/ja_JP/xs2ps.html) — 输出到 PS 文件的图形。
    *   [xs2svg](http://help.scilab.org/docs/5.4.0/ja_JP/xs2svg.html) — 对 SVG 文件的输出图形。

*   图形用户接口[GUI](http://help.scilab.org/docs/5.4.0/ja_JP/section_7ee063755077b27a8aa68306bd2a2f50.html)

    *   [Tree](http://help.scilab.org/docs/5.4.0/ja_JP/section_c10765d388fd01e759796942dd8b69fb.html)

            *   [uiConcatTree](http://help.scilab.org/docs/5.4.0/ja_JP/uiConcatTree.html) — 加入树
        *   [uiCreateNode](http://help.scilab.org/docs/5.4.0/ja_JP/uiCreateNode.html) — 创建一个节点 （对于 Scilab 树)
        *   [uiCreateTree](http://help.scilab.org/docs/5.4.0/ja_JP/uiCreateTree.html) — 创建一个目录树
        *   [uiDeleteNode](http://help.scilab.org/docs/5.4.0/ja_JP/uiDeleteNode.html) — 删除目录树
        *   [uiDisplayTree](http://help.scilab.org/docs/5.4.0/ja_JP/uiDisplayTree.html) — 打印在 GUI 模式下树
        *   [uiDumpTree](http://help.scilab.org/docs/5.4.0/ja_JP/uiDumpTree.html) — 打印的目录树中的控制台 （文本模式）
        *   [uiEqualsTree](http://help.scilab.org/docs/5.4.0/ja_JP/uiEqualsTree.html) — 比较两棵树
        *   [uiFindNode](http://help.scilab.org/docs/5.4.0/ja_JP/uiFindNode.html) — 在树中查找节点
        *   [uiGetChildrenNode](http://help.scilab.org/docs/5.4.0/ja_JP/uiGetChildrenNode.html) — 获取节点的子
        *   [uiGetNodePosition](http://help.scilab.org/docs/5.4.0/ja_JP/uiGetNodePosition.html) — 获取节点的位置
        *   [uiGetParentNode](http://help.scilab.org/docs/5.4.0/ja_JP/uiGetParentNode.html) — 获取父节点
        *   [uiInsertNode](http://help.scilab.org/docs/5.4.0/ja_JP/uiInsertNode.html) — 插入树

        *   [about](http://help.scilab.org/docs/5.4.0/ja_JP/about.html) — 请参阅"关于 scilab"对话框
    *   [addmenu](http://help.scilab.org/docs/5.4.0/ja_JP/addmenu.html) — 以交互方式定义按钮菜单中
    *   [clipboard](http://help.scilab.org/docs/5.4.0/ja_JP/clipboard.html) — 在系统剪贴板上 （或转出） 复制 / 粘贴。
    *   [close](http://help.scilab.org/docs/5.4.0/ja_JP/close.html) — 密切关系图
    *   [delmenu](http://help.scilab.org/docs/5.4.0/ja_JP/delmenu.html) — 删除交互式按钮/菜单
    *   [exportUI](http://help.scilab.org/docs/5.4.0/ja_JP/exportUI.html) — 要为 ファイルエキスポート 调用图形界面
    *   [figure](http://help.scilab.org/docs/5.4.0/ja_JP/figure.html) — 若要创建图表
    *   [findobj](http://help.scilab.org/docs/5.4.0/ja_JP/findobj.html) — 查找具有指定的属性的对象
    *   [gcbo](http://help.scilab.org/docs/5.4.0/ja_JP/gcbo.html) — 同时执行的回调对象句柄
    *   [getcallbackobject](http://help.scilab.org/docs/5.4.0/ja_JP/getcallbackobject.html) — 返回对象的回调的句的柄。
    *   [getinstalledlookandfeels](http://help.scilab.org/docs/5.4.0/ja_JP/getinstalledlookandfeels.html) — 返回一个字符串矩阵表示外观和感觉。
    *   [getlookandfeel](http://help.scilab.org/docs/5.4.0/ja_JP/getlookandfeel.html) — 获取当前的默认外观和感觉。
    *   [getvalue](http://help.scilab.org/docs/5.4.0/ja_JP/getvalue.html) — 数据检索的 Xwindow 对话框
    *   [messagebox](http://help.scilab.org/docs/5.4.0/ja_JP/messagebox.html) — 打开一个消息框。
    *   [printfigure](http://help.scilab.org/docs/5.4.0/ja_JP/printfigure.html) — 打开打印对话框打印关系图 ；
    *   [printsetupbox](http://help.scilab.org/docs/5.4.0/ja_JP/printsetupbox.html) — 若要显示打印对话框。
    *   [progressionbar](http://help.scilab.org/docs/5.4.0/ja_JP/progressionbar.html) — 绘制进度栏
    *   [root_properties](http://help.scilab.org/docs/5.4.0/ja_JP/root_properties.html) — 根对象属性的说明。
    *   [setlookandfeel](http://help.scilab.org/docs/5.4.0/ja_JP/setlookandfeel.html) — 设置的默认值为当前的外观和感觉。
    *   [setmenu](http://help.scilab.org/docs/5.4.0/ja_JP/setmenu.html) — 交互式按钮 / 菜单启用
    *   [toolbar](http://help.scilab.org/docs/5.4.0/ja_JP/toolbar.html) — 隐藏或显示工具栏
    *   [toprint](http://help.scilab.org/docs/5.4.0/ja_JP/toprint.html) — 向打印机发送文本或图形。
    *   [tree_show](http://help.scilab.org/docs/5.4.0/ja_JP/tree_show.html) — 若要显示树视图列表
    *   [uicontextmenu](http://help.scilab.org/docs/5.4.0/ja_JP/uicontextmenu.html) — 创建上下文菜单
    *   [uicontrol](http://help.scilab.org/docs/5.4.0/ja_JP/uicontrol.html) — 创建一个图形用户界面对象
    *   [uigetcolor](http://help.scilab.org/docs/5.4.0/ja_JP/uigetcolor.html) — 打开对话框中，选择一种颜色。
    *   [uigetdir](http://help.scilab.org/docs/5.4.0/ja_JP/uigetdir.html) — 选择目录对话框
    *   [uigetfile](http://help.scilab.org/docs/5.4.0/ja_JP/uigetfile.html) — 对话框窗口的文件的名称，路径，过滤为下标信
    *   [uigetfont](http://help.scilab.org/docs/5.4.0/ja_JP/uigetfont.html) — 打开字体选择对话框。
    *   [uimenu](http://help.scilab.org/docs/5.4.0/ja_JP/uimenu.html) — 若要创建菜单或子菜单图
    *   [uiputfile](http://help.scilab.org/docs/5.4.0/ja_JP/uiputfile.html) — 打开对话框中选择文件 / 保存的标准。
    *   [unsetmenu](http://help.scilab.org/docs/5.4.0/ja_JP/unsetmenu.html) — 交互式按钮或菜单中禁用
    *   [usecanvas](http://help.scilab.org/docs/5.4.0/ja_JP/usecanvas.html) — 获取或设置用于 Scilab 图形的主要元素。
    *   [waitbar](http://help.scilab.org/docs/5.4.0/ja_JP/waitbar.html) — 绘制 waitbar
    *   [x_choices](http://help.scilab.org/docs/5.4.0/ja_JP/x_choices.html) — 做出选择在切换按钮启用交互式 Xwindow
    *   [x_choose](http://help.scilab.org/docs/5.4.0/ja_JP/x_choose.html) — 交互式选择窗口 （模态对话框）
    *   [x_choose_modeless](http://help.scilab.org/docs/5.4.0/ja_JP/x_choose_modeless.html) — 交互式选择窗口 （不是模态对话框）
    *   [x_dialog](http://help.scilab.org/docs/5.4.0/ja_JP/x_dialog.html) — 交互式多行输入的对话框。
    *   [x_matrix](http://help.scilab.org/docs/5.4.0/ja_JP/x_matrix.html) — Xwindow 编辑矩阵
    *   [x_mdialog](http://help.scilab.org/docs/5.4.0/ja_JP/x_mdialog.html) — 矢量 / 矩阵的交互式对话框的输入。

*   数据结构[Data Structures](http://help.scilab.org/docs/5.4.0/ja_JP/section_e121e3e2a4638105da45968985f9c9a9.html)

    *   [boolean](http://help.scilab.org/docs/5.4.0/ja_JP/boolean.html) — Scilab 对象，（布尔） 布尔变量和运算符
    *   [cell](http://help.scilab.org/docs/5.4.0/ja_JP/cell.html) — 若要创建一个空白的矩阵单元格数组。
    *   [definedfields](http://help.scilab.org/docs/5.4.0/ja_JP/definedfields.html) — 返回的字段值列表是预定义的后缀
    *   [fieldnames](http://help.scilab.org/docs/5.4.0/ja_JP/fieldnames.html) — 获取或设置的 tlist、 mlist 或结构的字段名称
    *   [getfield](http://help.scilab.org/docs/5.4.0/ja_JP/getfield.html) — 列表中的字段的发展
    *   [hypermat](http://help.scilab.org/docs/5.4.0/ja_JP/hypermat.html) — 要初始化 N 维矩阵
    *   [hypermatrices](http://help.scilab.org/docs/5.4.0/ja_JP/hypermatrices.html) — Scilab 对象，Scilab 的 N 维矩阵
    *   [iscell](http://help.scilab.org/docs/5.4.0/ja_JP/iscell.html) — 确定是否变量是一个数组的单元格
    *   [iscellstr](http://help.scilab.org/docs/5.4.0/ja_JP/iscellstr.html) — 找出一个变量是否是字符串的单元格数组
    *   [isfield](http://help.scilab.org/docs/5.4.0/ja_JP/isfield.html) — 找出您所指定的字段名称是否在结构内
    *   [isstruct](http://help.scilab.org/docs/5.4.0/ja_JP/isstruct.html) — 找出一个变量是否是一个结构数组
    *   [list](http://help.scilab.org/docs/5.4.0/ja_JP/list.html) — 函数定义和 Scilab 对象的列表
    *   [lsslist](http://help.scilab.org/docs/5.4.0/ja_JP/lsslist.html) — 定义 Scilab 线性状态空间函数
    *   [lstcat](http://help.scilab.org/docs/5.4.0/ja_JP/lstcat.html) — 加入列表
    *   [matrices](http://help.scilab.org/docs/5.4.0/ja_JP/matrices.html) — Scilab 对象，Scilab 的矩阵
    *   [mlist](http://help.scilab.org/docs/5.4.0/ja_JP/mlist.html) — 适合 Scilab 对象，键入的列表定义的矩阵。
    *   [null](http://help.scilab.org/docs/5.4.0/ja_JP/null.html) — 若要删除列表的元素
    *   [rlist](http://help.scilab.org/docs/5.4.0/ja_JP/rlist.html) — Scilab 有理函数定义
    *   [setfield](http://help.scilab.org/docs/5.4.0/ja_JP/setfield.html) — 插入列表字段
    *   [struct](http://help.scilab.org/docs/5.4.0/ja_JP/struct.html) — 要创建的结构
    *   [tlist](http://help.scilab.org/docs/5.4.0/ja_JP/tlist.html) — Scilab 对象和类型的列表定义。
    *   [type](http://help.scilab.org/docs/5.4.0/ja_JP/type.html) — 返回变量的类型
    *   [typename](http://help.scilab.org/docs/5.4.0/ja_JP/typename.html) — 为名称的变量的类型
    *   [typeof](http://help.scilab.org/docs/5.4.0/ja_JP/typeof.html) — 对象的类型

*   参数[Parameters](http://help.scilab.org/docs/5.4.0/ja_JP/section_906004b5e0ef455f9dafe2ccb3bb6754.html)

    *   [add_param](http://help.scilab.org/docs/5.4.0/ja_JP/add_param.html) — 将参数添加到参数列表
    *   [get_param](http://help.scilab.org/docs/5.4.0/ja_JP/get_param.html) — 从参数列表中获取参数值
    *   [init_param](http://help.scilab.org/docs/5.4.0/ja_JP/init_param.html) — 初始化处理参数列表的结构
    *   [is_param](http://help.scilab.org/docs/5.4.0/ja_JP/is_param.html) — 请检查参数是否存在的参数列表中
    *   [list_param](http://help.scilab.org/docs/5.4.0/ja_JP/list_param.html) — 在参数列表中获取参数名称的列表
    *   [remove_param](http://help.scilab.org/docs/5.4.0/ja_JP/remove_param.html) — 从参数列表中移除的参数，其值
    *   [set_param](http://help.scilab.org/docs/5.4.0/ja_JP/set_param.html) — 要设置的参数列表中的参数的值

*   布尔[Boolean](http://help.scilab.org/docs/5.4.0/ja_JP/section_55e2d97c0fd248e3b2351deb07f8d72c.html)

    *   [bool2s](http://help.scilab.org/docs/5.4.0/ja_JP/bool2s.html) — 逻辑的矩阵 0，转换矩阵值为 1。
    *   [find](http://help.scilab.org/docs/5.4.0/ja_JP/find.html) — 查找 true 的元素的第一个下标的逻辑向量或矩阵

*   整数[Integers](http://help.scilab.org/docs/5.4.0/ja_JP/section_384944d2e569a2c1a8dfe0ee49b81cc1.html)

    *   [iconvert](http://help.scilab.org/docs/5.4.0/ja_JP/iconvert.html) — 1 或 4 字节的整数表示形式转换
    *   [int8](http://help.scilab.org/docs/5.4.0/ja_JP/int8.html) — 到 4 字节无符号的整数格式
    *   [inttype](http://help.scilab.org/docs/5.4.0/ja_JP/inttype.html) — 用于整数数据类型的整数类型

*   字符串[Strings](http://help.scilab.org/docs/5.4.0/ja_JP/section_b3813aece737943adef106cb67f9c83a.html)

    *   [ascii](http://help.scilab.org/docs/5.4.0/ja_JP/ascii.html) — 将 ASCII 转换为字符串
    *   [blanks](http://help.scilab.org/docs/5.4.0/ja_JP/blanks.html) — 若要创建由空格字符组成的字符串
    *   [char](http://help.scilab.org/docs/5.4.0/ja_JP/char.html) — char 函数
    *   [convstr](http://help.scilab.org/docs/5.4.0/ja_JP/convstr.html) — 大小写转换
    *   [emptystr](http://help.scilab.org/docs/5.4.0/ja_JP/emptystr.html) — 一个字符串，长度为 0 的
    *   [eval](http://help.scilab.org/docs/5.4.0/ja_JP/eval.html) — 矩阵的字符串的评价
    *   [evstr](http://help.scilab.org/docs/5.4.0/ja_JP/evstr.html) — 表达式的计算
    *   [grep](http://help.scilab.org/docs/5.4.0/ja_JP/grep.html) — 查找匹配的字符串向量中的字符串
    *   [isalphanum](http://help.scilab.org/docs/5.4.0/ja_JP/isalphanum.html) — 找出字符的字符串是否是数字或字母列表中
    *   [isascii](http://help.scilab.org/docs/5.4.0/ja_JP/isascii.html) — 要确定中美国 ASCII 字符字符的 7 位
    *   [isdigit](http://help.scilab.org/docs/5.4.0/ja_JP/isdigit.html) — 字符的字符串是介于 0 和找出是否之间的数字 9
    *   [isletter](http://help.scilab.org/docs/5.4.0/ja_JP/isletter.html) — 确定字符串的字符是否为字母字符
    *   [isnum](http://help.scilab.org/docs/5.4.0/ja_JP/isnum.html) — 确定字符串是否是数字
    *   [justify](http://help.scilab.org/docs/5.4.0/ja_JP/justify.html) — 排队的字符数组。
    *   [length](http://help.scilab.org/docs/5.4.0/ja_JP/length.html) — 对象的长度
    *   [part](http://help.scilab.org/docs/5.4.0/ja_JP/part.html) — 字符串扩展
    *   [regexp](http://help.scilab.org/docs/5.4.0/ja_JP/regexp.html) — 搜索匹配的正则表达式字符串的子字符串
    *   [sci2exp](http://help.scilab.org/docs/5.4.0/ja_JP/sci2exp.html) — 将转换为字符串
    *   [strcat](http://help.scilab.org/docs/5.4.0/ja_JP/strcat.html) — 若要将文本与合并
    *   [strchr](http://help.scilab.org/docs/5.4.0/ja_JP/strchr.html) — 第一次出现的指定字符串中的字符查找位置
    *   [strcmp](http://help.scilab.org/docs/5.4.0/ja_JP/strcmp.html) — 比较字符串
    *   [strcmpi](http://help.scilab.org/docs/5.4.0/ja_JP/strcmpi.html) — 比较字符串 （视情况）
    *   [strcspn](http://help.scilab.org/docs/5.4.0/ja_JP/strcspn.html) — 获取字符串中的字符之间的距离
    *   [strindex](http://help.scilab.org/docs/5.4.0/ja_JP/strindex.html) — 查找一个字符串在另一个字符串内的位置。
    *   [string](http://help.scilab.org/docs/5.4.0/ja_JP/string.html) — 将转换为字符串
    *   [strings](http://help.scilab.org/docs/5.4.0/ja_JP/strings.html) — Scilab 对象字符串
    *   [stripblanks](http://help.scilab.org/docs/5.4.0/ja_JP/stripblanks.html) — 摆脱的开头或结尾的字符串空间 (およびタブ)
    *   [strncpy](http://help.scilab.org/docs/5.4.0/ja_JP/strncpy.html) — 从字符串复制字符
    *   [strrchr](http://help.scilab.org/docs/5.4.0/ja_JP/strrchr.html) — 搜索字符串中的字符的最后一个匹配项
    *   [strrev](http://help.scilab.org/docs/5.4.0/ja_JP/strrev.html) — 返回的反转文本
    *   [strsplit](http://help.scilab.org/docs/5.4.0/ja_JP/strsplit.html) — 以字符串分成一个字符串向量
    *   [strspn](http://help.scilab.org/docs/5.4.0/ja_JP/strspn.html) — 获取指定字符串中的字符设置的宽度
    *   [strstr](http://help.scilab.org/docs/5.4.0/ja_JP/strstr.html) — 获取子字符串
    *   [strsubst](http://help.scilab.org/docs/5.4.0/ja_JP/strsubst.html) — 若要用其他文本替换文本。
    *   [strtod](http://help.scilab.org/docs/5.4.0/ja_JP/strtod.html) — 将字符串转换为双精度实数。
    *   [strtok](http://help.scilab.org/docs/5.4.0/ja_JP/strtok.html) — 将字符串拆分为标记
    *   [tokenpos](http://help.scilab.org/docs/5.4.0/ja_JP/tokenpos.html) — 返回字符串中的位置的标记。
    *   [tokens](http://help.scilab.org/docs/5.4.0/ja_JP/tokens.html) — 返回的字符串标记。

*   声音文件处理[Sound file handling](http://help.scilab.org/docs/5.4.0/ja_JP/section_65171486c4fd6170d5512de46dfd7922.html)

    *   [analyze](http://help.scilab.org/docs/5.4.0/ja_JP/analyze.html) — 频率的声音信号的阴谋
    *   [auread](http://help.scilab.org/docs/5.4.0/ja_JP/auread.html) — load.au 声音文件
    *   [auwrite](http://help.scilab.org/docs/5.4.0/ja_JP/auwrite.html) — writes.au 声音文件
    *   [beep](http://help.scilab.org/docs/5.4.0/ja_JP/beep.html) — 产生蜂鸣声
    *   [lin2mu](http://help.scilab.org/docs/5.4.0/ja_JP/lin2mu.html) — 线性信号到亩法编码
    *   [loadwave](http://help.scilab.org/docs/5.4.0/ja_JP/loadwave.html) — 声音 wav 文件加载到 scilab
    *   [mapsound](http://help.scilab.org/docs/5.4.0/ja_JP/mapsound.html) — 地块声音地图
    *   [mu2lin](http://help.scilab.org/docs/5.4.0/ja_JP/mu2lin.html) — 穆法向线性信号编码
    *   [playsnd](http://help.scilab.org/docs/5.4.0/ja_JP/playsnd.html) — 声音播放机设施
    *   [savewave](http://help.scilab.org/docs/5.4.0/ja_JP/savewave.html) — 将数据保存到一个声音 wav 文件。
    *   [sound](http://help.scilab.org/docs/5.4.0/ja_JP/sound.html) — 声音播放机设施
    *   [soundsec](http://help.scilab.org/docs/5.4.0/ja_JP/soundsec.html) — 生成 n 采样的秒的时间参数
    *   [wavread](http://help.scilab.org/docs/5.4.0/ja_JP/wavread.html) — load.wav 声音文件
    *   [wavwrite](http://help.scilab.org/docs/5.4.0/ja_JP/wavwrite.html) — writes.wav 声音文件

*   时间和日期[Time and Date](http://help.scilab.org/docs/5.4.0/ja_JP/section_502575311db3ddfb7ba3aaac8a79e105.html)

    *   [calendar](http://help.scilab.org/docs/5.4.0/ja_JP/calendar.html) — 日历
    *   [clock](http://help.scilab.org/docs/5.4.0/ja_JP/clock.html) — 返回当前时间作为日期矢量
    *   [date](http://help.scilab.org/docs/5.4.0/ja_JP/date.html) — 获取当前日期作为日期字符串
    *   [datenum](http://help.scilab.org/docs/5.4.0/ja_JP/datenum.html) — 转换日期的序列数
    *   [datevec](http://help.scilab.org/docs/5.4.0/ja_JP/datevec.html) — 日期元素
    *   [eomday](http://help.scilab.org/docs/5.4.0/ja_JP/eomday.html) — 返回该月的最后一天
    *   [etime](http://help.scilab.org/docs/5.4.0/ja_JP/etime.html) — 经过的时间
    *   [getdate](http://help.scilab.org/docs/5.4.0/ja_JP/getdate.html) — 获取有关的日期和时间信息
    *   [now](http://help.scilab.org/docs/5.4.0/ja_JP/now.html) — 返回当前日期和时间
    *   [realtime](http://help.scilab.org/docs/5.4.0/ja_JP/realtime.html) — 等待日期起源配置或指定的日期
    *   [sleep](http://help.scilab.org/docs/5.4.0/ja_JP/sleep.html) — 停止 Scilab （暂停）
    *   [tic](http://help.scilab.org/docs/5.4.0/ja_JP/tic.html) — 启动秒表计时器
    *   [timer](http://help.scilab.org/docs/5.4.0/ja_JP/timer.html) — CPU 时间
    *   [toc](http://help.scilab.org/docs/5.4.0/ja_JP/toc.html) — 读取秒表计时器
    *   [weekday](http://help.scilab.org/docs/5.4.0/ja_JP/weekday.html) — 返回星期中的第几天

*   输出[Output functions](http://help.scilab.org/docs/5.4.0/ja_JP/section_5de38aabd85ccbc33a8612378939e0db.html)

    *   [disp](http://help.scilab.org/docs/5.4.0/ja_JP/disp.html) — 显示变量
    *   [mprintf](http://help.scilab.org/docs/5.4.0/ja_JP/mprintf.html) — 转换、 设置格式和数据写入主 Scilab 窗口
    *   [msprintf](http://help.scilab.org/docs/5.4.0/ja_JP/msprintf.html) — 将数据转换、 写入字符串格式
    *   [prettyprint](http://help.scilab.org/docs/5.4.0/ja_JP/prettyprint.html) — Scilab 的数据类型从获取 TeX、 乳胶或 MathML 的格式输出
    *   [print](http://help.scilab.org/docs/5.4.0/ja_JP/print.html) — 变量输出文件
    *   [printf_conversion](http://help.scilab.org/docs/5.4.0/ja_JP/printf_conversion.html) — mprintf，msprintf，mfprintf 的转换规范

*   [Xcos](http://help.scilab.org/docs/5.4.0/ja_JP/section_73836daae3b0a6277011912dd615f820.html)

    *   [Batch functions](http://help.scilab.org/docs/5.4.0/ja_JP/section_53a16c8ff2bddef53e995e7ed377dc15.html)

            *   [lincos](http://help.scilab.org/docs/5.4.0/ja_JP/lincos.html) — 由图 xcos 线性状态空间模型所描述的一般动力系统的线性化定义
        *   [scicos](http://help.scilab.org/docs/5.4.0/ja_JP/scicos.html) — Xcos 已过时的见
        *   [scicos_simulate](http://help.scilab.org/docs/5.4.0/ja_JP/scicos_simulate.html) — 在批处理模式下执行模拟的职能
        *   [scicosim](http://help.scilab.org/docs/5.4.0/ja_JP/scicosim.html) — xcos (批) 仿真功能
        *   [steadycos](http://help.scilab.org/docs/5.4.0/ja_JP/steadycos.html) — 查找状态变量一般动力系统由 xcos 图中描述的稳态值
        *   [xcosValidateBlockSet](http://help.scilab.org/docs/5.4.0/ja_JP/xcosValidateBlockSet.html) — 要验证 Xcos 块接口函数的函数。
        *   [xcosValidateCompareBlock](http://help.scilab.org/docs/5.4.0/ja_JP/xcosValidateCompareBlock.html) — 一个函数，比较 2 Xcos 块。
        *   [xcos_simulate](http://help.scilab.org/docs/5.4.0/ja_JP/xcos_simulate.html) — 在批处理模式下执行 xcos 仿真的职能

        *   [scilab_data_structures](http://help.scilab.org/docs/5.4.0/ja_JP/section_da07de1d2564e4b9396d7bb86ee2ab40.html)

            *   [Blocks](http://help.scilab.org/docs/5.4.0/ja_JP/section_3f3a4dfa62dd7e2017e932cf01c12755.html)

                    *   [scicos_block](http://help.scilab.org/docs/5.4.0/ja_JP/scicos_block.html) — 定义块结构
            *   [scicos_graphics](http://help.scilab.org/docs/5.4.0/ja_JP/scicos_graphics.html) — 定义图形
            *   [scicos_model](http://help.scilab.org/docs/5.4.0/ja_JP/scicos_model.html) — 定义模型的结构

                *   [Compilation/Simulation](http://help.scilab.org/docs/5.4.0/ja_JP/section_4fcd5605265c5fcbd7cb6b997ed1ca38.html)

                    *   [scicos_cpr](http://help.scilab.org/docs/5.4.0/ja_JP/scicos_cpr.html) — 编译的 Scicos 结构
            *   [scicos_sim](http://help.scilab.org/docs/5.4.0/ja_JP/scicos_sim.html) — 定义一个 sim 卡结构
            *   [scicos_state](http://help.scilab.org/docs/5.4.0/ja_JP/scicos_state.html) — 定义状态结构

                *   [Diagram](http://help.scilab.org/docs/5.4.0/ja_JP/section_c5ed49f87c3013a765770e5ea10b2d78.html)

                    *   [scicos_diagram](http://help.scilab.org/docs/5.4.0/ja_JP/scicos_diagram.html) — 定义一个 scs_m 结构
            *   [scicos_params](http://help.scilab.org/docs/5.4.0/ja_JP/scicos_params.html) — 定义参数的结构

                *   [Links](http://help.scilab.org/docs/5.4.0/ja_JP/section_4c9b198431fc3d7cb382c64da3847197.html)

                    *   [scicos_link](http://help.scilab.org/docs/5.4.0/ja_JP/scicos_link.html) — 定义链接结构

        *   [palettes](http://help.scilab.org/docs/5.4.0/ja_JP/section_4834819644bddf2dedeef2520b2ca171.html)

            *   [Annotations palette](http://help.scilab.org/docs/5.4.0/ja_JP/section_6294dbe5e43b9ef27c5b5345a37edb6d.html)

                    *   [Annotations_pal](http://help.scilab.org/docs/5.4.0/ja_JP/Annotations_pal.html) — 批注调色板
            *   [TEXT_f](http://help.scilab.org/docs/5.4.0/ja_JP/TEXT_f.html) — 自由的批注

                *   [Commonly used blocks palette](http://help.scilab.org/docs/5.4.0/ja_JP/section_c19d6dbe42e82a00027e775138035986.html)

                    *   [Commonlyusedblocks_pal](http://help.scilab.org/docs/5.4.0/ja_JP/Commonlyusedblocks_pal.html) — 常用块调色板
            *   [LOGICAL_OP](http://help.scilab.org/docs/5.4.0/ja_JP/LOGICAL_OP.html) — 逻辑操作
            *   [RELATIONALOP](http://help.scilab.org/docs/5.4.0/ja_JP/RELATIONALOP.html) — 关系操作

                *   [Continuous time systems palette](http://help.scilab.org/docs/5.4.0/ja_JP/section_10261ac2c63340e6a753699961fb03f4.html)

                    *   [Continuous_pal](http://help.scilab.org/docs/5.4.0/ja_JP/Continuous_pal.html) — 连续时间系统调色板
            *   [CLINDUMMY_f](http://help.scilab.org/docs/5.4.0/ja_JP/CLINDUMMY_f.html) — 虚拟
            *   [CLR](http://help.scilab.org/docs/5.4.0/ja_JP/CLR.html) — 连续传递函数
            *   [CLSS](http://help.scilab.org/docs/5.4.0/ja_JP/CLSS.html) — 连续状态空间系统
            *   [DERIV](http://help.scilab.org/docs/5.4.0/ja_JP/DERIV.html) — 导数
            *   [INTEGRAL_f](http://help.scilab.org/docs/5.4.0/ja_JP/INTEGRAL_f.html) — 一体化
            *   [INTEGRAL_m](http://help.scilab.org/docs/5.4.0/ja_JP/INTEGRAL_m.html) — 一体化
            *   [PID](http://help.scilab.org/docs/5.4.0/ja_JP/PID.html) — PID 调节器
            *   [TCLSS](http://help.scilab.org/docs/5.4.0/ja_JP/TCLSS.html) — 连续线性系统的跳转
            *   [TIME_DELAY](http://help.scilab.org/docs/5.4.0/ja_JP/TIME_DELAY.html) — 延迟时间
            *   [VARIABLE_DELAY](http://help.scilab.org/docs/5.4.0/ja_JP/VARIABLE_DELAY.html) — 可变时滞

                *   [Demonstrations blocks palette](http://help.scilab.org/docs/5.4.0/ja_JP/section_46ed7769d76fa28f6c1cc06d04ff053c.html)

                    *   [Demonstrationsblocks_pal](http://help.scilab.org/docs/5.4.0/ja_JP/Demonstrationsblocks_pal.html) — 示威活动块调色板
            *   [AUTOMAT](http://help.scilab.org/docs/5.4.0/ja_JP/AUTOMAT.html) — 自动机 (有限状态机)
            *   [BOUNCE](http://help.scilab.org/docs/5.4.0/ja_JP/BOUNCE.html) — 球坐标发电机
            *   [BOUNCEXY](http://help.scilab.org/docs/5.4.0/ja_JP/BOUNCEXY.html) — 球查看器
            *   [BPLATFORM](http://help.scilab.org/docs/5.4.0/ja_JP/BPLATFORM.html) — 根据平台查看器球
            *   [PDE](http://help.scilab.org/docs/5.4.0/ja_JP/PDE.html) — 1 D PDE 块

                *   [Discontinuities palette](http://help.scilab.org/docs/5.4.0/ja_JP/section_97397af3277b341e12ea7bc8dca25242.html)

                    *   [discontinuities_pal](http://help.scilab.org/docs/5.4.0/ja_JP/discontinuities_pal.html) — 不连续性调色板
            *   [BACKLASH](http://help.scilab.org/docs/5.4.0/ja_JP/BACKLASH.html) — 反弹
            *   [DEADBAND](http://help.scilab.org/docs/5.4.0/ja_JP/DEADBAND.html) — 死区
            *   [HYSTHERESIS](http://help.scilab.org/docs/5.4.0/ja_JP/HYSTHERESIS.html) — Hystheresis
            *   [RATELIMITER](http://help.scilab.org/docs/5.4.0/ja_JP/RATELIMITER.html) — 速率限制器
            *   [SATURATION](http://help.scilab.org/docs/5.4.0/ja_JP/SATURATION.html) — 饱和度

                *   [Discrete time systems palette](http://help.scilab.org/docs/5.4.0/ja_JP/section_b3122376069b7df39e6b511b99065527.html)

                    *   [Discrete_pal](http://help.scilab.org/docs/5.4.0/ja_JP/Discrete_pal.html) — 离散时间系统调色板
            *   [DELAYV_f](http://help.scilab.org/docs/5.4.0/ja_JP/DELAYV_f.html) — 可变时滞
            *   [DELAY_f](http://help.scilab.org/docs/5.4.0/ja_JP/DELAY_f.html) — 离散时的延迟时间
            *   [DLR](http://help.scilab.org/docs/5.4.0/ja_JP/DLR.html) — 离散传递函数
            *   [DLRADAPT_f](http://help.scilab.org/docs/5.4.0/ja_JP/DLRADAPT_f.html) — 离散的零极点
            *   [DLSS](http://help.scilab.org/docs/5.4.0/ja_JP/DLSS.html) — 离散状态空间系统
            *   [DOLLAR_f](http://help.scilab.org/docs/5.4.0/ja_JP/DOLLAR_f.html) — 延迟运算符
            *   [REGISTER](http://help.scilab.org/docs/5.4.0/ja_JP/REGISTER.html) — 移位寄存器

                *   [Electrical palette](http://help.scilab.org/docs/5.4.0/ja_JP/section_9f0b6ef9735a0eb9e08461f8fdaa2426.html)

                    *   [Electrical_pal](http://help.scilab.org/docs/5.4.0/ja_JP/Electrical_pal.html) — 电气调色板
            *   [CCS](http://help.scilab.org/docs/5.4.0/ja_JP/CCS.html) — 可控 Modelica 当前源
            *   [CVS](http://help.scilab.org/docs/5.4.0/ja_JP/CVS.html) — 可控 Modelica 电压源
            *   [Capacitor](http://help.scilab.org/docs/5.4.0/ja_JP/Capacitor.html) — 电力电容器
            *   [ConstantVoltage](http://help.scilab.org/docs/5.4.0/ja_JP/ConstantVoltage.html) — 电气直流电压源
            *   [CurrentSensor](http://help.scilab.org/docs/5.4.0/ja_JP/CurrentSensor.html) — 电气电流传感器
            *   [Diode](http://help.scilab.org/docs/5.4.0/ja_JP/Diode.html) — 电二极管
            *   [Ground](http://help.scilab.org/docs/5.4.0/ja_JP/Ground.html) — 地面 （零潜在的参考）
            *   [Gyrator](http://help.scilab.org/docs/5.4.0/ja_JP/Gyrator.html) — Modelica 回转器
            *   [IdealTransformer](http://help.scilab.org/docs/5.4.0/ja_JP/IdealTransformer.html) — 理想变压器
            *   [Inductor](http://help.scilab.org/docs/5.4.0/ja_JP/Inductor.html) — 电气电感器
            *   [NMOS](http://help.scilab.org/docs/5.4.0/ja_JP/NMOS.html) — 简单 NMOS 晶体管
            *   [NPN](http://help.scilab.org/docs/5.4.0/ja_JP/NPN.html) — NPN 晶体管
            *   [OpAmp](http://help.scilab.org/docs/5.4.0/ja_JP/OpAmp.html) — 理想运放 （norator-nullator pair）
            *   [PMOS](http://help.scilab.org/docs/5.4.0/ja_JP/PMOS.html) — 简单的 PMOS 晶体管
            *   [PNP](http://help.scilab.org/docs/5.4.0/ja_JP/PNP.html) — PNP 晶体管
            *   [PotentialSensor](http://help.scilab.org/docs/5.4.0/ja_JP/PotentialSensor.html) — 潜在的传感器
            *   [Resistor](http://help.scilab.org/docs/5.4.0/ja_JP/Resistor.html) — 电气电阻
            *   [SineVoltage](http://help.scilab.org/docs/5.4.0/ja_JP/SineVoltage.html) — 正弦电压源
            *   [Switch](http://help.scilab.org/docs/5.4.0/ja_JP/Switch.html) — 在非理想电气开关
            *   [VVsourceAC](http://help.scilab.org/docs/5.4.0/ja_JP/VVsourceAC.html) — 可变的交流电压源
            *   [VariableResistor](http://help.scilab.org/docs/5.4.0/ja_JP/VariableResistor.html) — 电气可变电阻器
            *   [VoltageSensor](http://help.scilab.org/docs/5.4.0/ja_JP/VoltageSensor.html) — 电电压传感器
            *   [VsourceAC](http://help.scilab.org/docs/5.4.0/ja_JP/VsourceAC.html) — 电气交流电压源

                *   [Event handling palette](http://help.scilab.org/docs/5.4.0/ja_JP/section_8942903e40195fa7f9e18de4f7e5b9b0.html)

                    *   [Events_pal](http://help.scilab.org/docs/5.4.0/ja_JP/Events_pal.html) — 事件处理调色板
            *   [ANDBLK](http://help.scilab.org/docs/5.4.0/ja_JP/ANDBLK.html) — 激活和
            *   [ANDLOG_f](http://help.scilab.org/docs/5.4.0/ja_JP/ANDLOG_f.html) — 逻辑和
            *   [CEVENTSCOPE](http://help.scilab.org/docs/5.4.0/ja_JP/CEVENTSCOPE.html) — 激活范围
            *   [CLKFROM](http://help.scilab.org/docs/5.4.0/ja_JP/CLKFROM.html) — 从相应的 CLKGOTO 接收数据
            *   [CLKGOTO](http://help.scilab.org/docs/5.4.0/ja_JP/CLKGOTO.html) — 将块输入传递给 CLKFROM 块
            *   [CLKGotoTagVisibility](http://help.scilab.org/docs/5.4.0/ja_JP/CLKGotoTagVisibility.html) — 定义范围的 CLKGOTO 标记可见性
            *   [CLKSOMV_f](http://help.scilab.org/docs/5.4.0/ja_JP/CLKSOMV_f.html) — 激活联盟
            *   [EDGE_TRIGGER](http://help.scilab.org/docs/5.4.0/ja_JP/EDGE_TRIGGER.html) — EDGE_TRIGGER 块
            *   [ESELECT_f](http://help.scilab.org/docs/5.4.0/ja_JP/ESELECT_f.html) — 同步块事件选择
            *   [EVTDLY_c](http://help.scilab.org/docs/5.4.0/ja_JP/EVTDLY_c.html) — 事件延迟
            *   [EVTGEN_f](http://help.scilab.org/docs/5.4.0/ja_JP/EVTGEN_f.html) — 事件发生器
            *   [EVTVARDLY](http://help.scilab.org/docs/5.4.0/ja_JP/EVTVARDLY.html) — 事件变量延迟
            *   [Extract_Activation](http://help.scilab.org/docs/5.4.0/ja_JP/Extract_Activation.html) — Extract_Activation 块
            *   [HALT_f](http://help.scilab.org/docs/5.4.0/ja_JP/HALT_f.html) — 停止
            *   [IFTHEL_f](http://help.scilab.org/docs/5.4.0/ja_JP/IFTHEL_f.html) — 如果那时其他同步块
            *   [MCLOCK_f](http://help.scilab.org/docs/5.4.0/ja_JP/MCLOCK_f.html) — MCLOCK_f 标题
            *   [MFCLCK_f](http://help.scilab.org/docs/5.4.0/ja_JP/MFCLCK_f.html) — MFCLCK_f 标题
            *   [M_freq](http://help.scilab.org/docs/5.4.0/ja_JP/M_freq.html) — 多个频率
            *   [VirtualCLK0](http://help.scilab.org/docs/5.4.0/ja_JP/VirtualCLK0.html) — 触发始终处于活动状态块
            *   [freq_div](http://help.scilab.org/docs/5.4.0/ja_JP/freq_div.html) — 频分

                *   [Implicit palette](http://help.scilab.org/docs/5.4.0/ja_JP/section_b2e6b114da18af56c93701716bcc227c.html)

                    *   [Implicit_pal](http://help.scilab.org/docs/5.4.0/ja_JP/Implicit_pal.html) — 隐式的调色板
            *   [CONSTRAINT_c](http://help.scilab.org/docs/5.4.0/ja_JP/CONSTRAINT_c.html) — 约束
            *   [DIFF_f](http://help.scilab.org/docs/5.4.0/ja_JP/DIFF_f.html) — 导数

                *   [Integer palette](http://help.scilab.org/docs/5.4.0/ja_JP/section_874cc4c61c9349af846c73f344feea18.html)

                    *   [Integer_pal](http://help.scilab.org/docs/5.4.0/ja_JP/Integer_pal.html) — 整数调色板
            *   [BITCLEAR](http://help.scilab.org/docs/5.4.0/ja_JP/BITCLEAR.html) — 有点清除
            *   [BITSET](http://help.scilab.org/docs/5.4.0/ja_JP/BITSET.html) — 设置有点
            *   [CONVERT](http://help.scilab.org/docs/5.4.0/ja_JP/CONVERT.html) — 数据类型转换
            *   [DFLIPFLOP](http://help.scilab.org/docs/5.4.0/ja_JP/DFLIPFLOP.html) — D 触发器
            *   [DLATCH](http://help.scilab.org/docs/5.4.0/ja_JP/DLATCH.html) — D 触发器
            *   [EXTRACTBITS](http://help.scilab.org/docs/5.4.0/ja_JP/EXTRACTBITS.html) — Bits 提取
            *   [INTMUL](http://help.scilab.org/docs/5.4.0/ja_JP/INTMUL.html) — 整数矩阵乘法
            *   [JKFLIPFLOP](http://help.scilab.org/docs/5.4.0/ja_JP/JKFLIPFLOP.html) — Jk
            *   [LOGIC](http://help.scilab.org/docs/5.4.0/ja_JP/LOGIC.html) — 组合逻辑
            *   [SHIFT](http://help.scilab.org/docs/5.4.0/ja_JP/SHIFT.html) — 旋转移位/位
            *   [SRFLIPFLOP](http://help.scilab.org/docs/5.4.0/ja_JP/SRFLIPFLOP.html) — SR 触发器

                *   [Lookup tables palette](http://help.scilab.org/docs/5.4.0/ja_JP/section_e5fb4c709d7d9eafc6c7418b5e19f674.html)

                    *   [Lookuptables_pal](http://help.scilab.org/docs/5.4.0/ja_JP/Lookuptables_pal.html) — 查找表调色板
            *   [INTRP2BLK_f](http://help.scilab.org/docs/5.4.0/ja_JP/INTRP2BLK_f.html) — 2D 插值
            *   [INTRPLBLK_f](http://help.scilab.org/docs/5.4.0/ja_JP/INTRPLBLK_f.html) — 插值
            *   [LOOKUP_f](http://help.scilab.org/docs/5.4.0/ja_JP/LOOKUP_f.html) — 查找表

                *   [Math operations palette](http://help.scilab.org/docs/5.4.0/ja_JP/section_91bfa65ee8cb0a4362885ee673742c4f.html)

                    *   [Mathoperations_pal](http://help.scilab.org/docs/5.4.0/ja_JP/Mathoperations_pal.html) — 数学操作调色板
            *   [ABS_VALUE](http://help.scilab.org/docs/5.4.0/ja_JP/ABS_VALUE.html) — 绝对值
            *   [BIGSOM_f](http://help.scilab.org/docs/5.4.0/ja_JP/BIGSOM_f.html) — 标量或矢量加法/Soustraction
            *   [COSBLK_f](http://help.scilab.org/docs/5.4.0/ja_JP/COSBLK_f.html) — 余弦
            *   [EXPBLK_m](http://help.scilab.org/docs/5.4.0/ja_JP/EXPBLK_m.html) — 指数的标量
            *   [GAINBLK_f](http://help.scilab.org/docs/5.4.0/ja_JP/GAINBLK_f.html) — 增益
            *   [INVBLK](http://help.scilab.org/docs/5.4.0/ja_JP/INVBLK.html) — 逆
            *   [LOGBLK_f](http://help.scilab.org/docs/5.4.0/ja_JP/LOGBLK_f.html) — 对数
            *   [MATMAGPHI](http://help.scilab.org/docs/5.4.0/ja_JP/MATMAGPHI.html) — 复杂从/的程度和角度转换
            *   [MATZREIM](http://help.scilab.org/docs/5.4.0/ja_JP/MATZREIM.html) — 每个组成复杂分解
            *   [MAXMIN](http://help.scilab.org/docs/5.4.0/ja_JP/MAXMIN.html) — 向量的元素的最大或最小值
            *   [MAX_f](http://help.scilab.org/docs/5.4.0/ja_JP/MAX_f.html) — 一个向量元素的最大值
            *   [MIN_f](http://help.scilab.org/docs/5.4.0/ja_JP/MIN_f.html) — 向量元素的最小值
            *   [POWBLK_f](http://help.scilab.org/docs/5.4.0/ja_JP/POWBLK_f.html) — 阵列电源
            *   [PRODUCT](http://help.scilab.org/docs/5.4.0/ja_JP/PRODUCT.html) — 聪明元素矢量乘法/司
            *   [PROD_f](http://help.scilab.org/docs/5.4.0/ja_JP/PROD_f.html) — 聪明元素产品
            *   [SIGNUM](http://help.scilab.org/docs/5.4.0/ja_JP/SIGNUM.html) — 登录
            *   [SINBLK_f](http://help.scilab.org/docs/5.4.0/ja_JP/SINBLK_f.html) — 正弦
            *   [SQRT](http://help.scilab.org/docs/5.4.0/ja_JP/SQRT.html) — 平方根
            *   [SUMMATION](http://help.scilab.org/docs/5.4.0/ja_JP/SUMMATION.html) — 矩阵加法/减法
            *   [SUM_f](http://help.scilab.org/docs/5.4.0/ja_JP/SUM_f.html) — 加法
            *   [TANBLK_f](http://help.scilab.org/docs/5.4.0/ja_JP/TANBLK_f.html) — 切线
            *   [TrigFun](http://help.scilab.org/docs/5.4.0/ja_JP/TrigFun.html) — 三角函数

                *   [Matrix operation palette](http://help.scilab.org/docs/5.4.0/ja_JP/section_f47154a531c2201353786a8450658145.html)

                    *   [Matrix_pal](http://help.scilab.org/docs/5.4.0/ja_JP/Matrix_pal.html) — 矩阵操作调色板
            *   [CUMSUM](http://help.scilab.org/docs/5.4.0/ja_JP/CUMSUM.html) — 累积总和
            *   [EXTRACT](http://help.scilab.org/docs/5.4.0/ja_JP/EXTRACT.html) — 矩阵提取器
            *   [EXTTRI](http://help.scilab.org/docs/5.4.0/ja_JP/EXTTRI.html) — 三角或对角线的提取
            *   [MATBKSL](http://help.scilab.org/docs/5.4.0/ja_JP/MATBKSL.html) — 左的矩阵司
            *   [MATCATH](http://help.scilab.org/docs/5.4.0/ja_JP/MATCATH.html) — 水平串联
            *   [MATCATV](http://help.scilab.org/docs/5.4.0/ja_JP/MATCATV.html) — 垂直串联
            *   [MATDET](http://help.scilab.org/docs/5.4.0/ja_JP/MATDET.html) — 矩阵行列式
            *   [MATDIAG](http://help.scilab.org/docs/5.4.0/ja_JP/MATDIAG.html) — 创建对角矩阵
            *   [MATDIV](http://help.scilab.org/docs/5.4.0/ja_JP/MATDIV.html) — 矩阵司
            *   [MATEIG](http://help.scilab.org/docs/5.4.0/ja_JP/MATEIG.html) — 矩阵特征值
            *   [MATEXPM](http://help.scilab.org/docs/5.4.0/ja_JP/MATEXPM.html) — 矩阵指数
            *   [MATINV](http://help.scilab.org/docs/5.4.0/ja_JP/MATINV.html) — 矩阵逆
            *   [MATLU](http://help.scilab.org/docs/5.4.0/ja_JP/MATLU.html) — LU 分解
            *   [MATMUL](http://help.scilab.org/docs/5.4.0/ja_JP/MATMUL.html) — 矩阵乘法
            *   [MATPINV](http://help.scilab.org/docs/5.4.0/ja_JP/MATPINV.html) — 矩阵伪逆法
            *   [MATRESH](http://help.scilab.org/docs/5.4.0/ja_JP/MATRESH.html) — 重塑一个矩阵
            *   [MATSING](http://help.scilab.org/docs/5.4.0/ja_JP/MATSING.html) — 奇异值分解
            *   [MATSUM](http://help.scilab.org/docs/5.4.0/ja_JP/MATSUM.html) — 矩阵的元素的总和
            *   [MATTRAN](http://help.scilab.org/docs/5.4.0/ja_JP/MATTRAN.html) — 矩阵的转置
            *   [MATZCONJ](http://help.scilab.org/docs/5.4.0/ja_JP/MATZCONJ.html) — 共轭矩阵的元素的
            *   [RICC](http://help.scilab.org/docs/5.4.0/ja_JP/RICC.html) — 黎卡提方程
            *   [ROOTCOEF](http://help.scilab.org/docs/5.4.0/ja_JP/ROOTCOEF.html) — 多项式系数计算
            *   [SUBMAT](http://help.scilab.org/docs/5.4.0/ja_JP/SUBMAT.html) — 子矩阵提取

                *   [Port &amp; Subsystem palette](http://help.scilab.org/docs/5.4.0/ja_JP/section_240c06a34eb8a41cb41176eb81a404cd.html)

                    *   [Portaction_pal](http://help.scilab.org/docs/5.4.0/ja_JP/Portaction_pal.html) — 端口
            *   [CLKINV_f](http://help.scilab.org/docs/5.4.0/ja_JP/CLKINV_f.html) — 激活输入的端口
            *   [CLKOUTV_f](http://help.scilab.org/docs/5.4.0/ja_JP/CLKOUTV_f.html) — 输出激活端口
            *   [INIMPL_f](http://help.scilab.org/docs/5.4.0/ja_JP/INIMPL_f.html) — 隐式输入端口
            *   [IN_f](http://help.scilab.org/docs/5.4.0/ja_JP/IN_f.html) — 经常输入端口
            *   [OUTIMPL_f](http://help.scilab.org/docs/5.4.0/ja_JP/OUTIMPL_f.html) — 隐式的输出端口
            *   [OUT_f](http://help.scilab.org/docs/5.4.0/ja_JP/OUT_f.html) — 定期输出端口

                *   [Signal processing palette](http://help.scilab.org/docs/5.4.0/ja_JP/section_e0f5b7fd0ef62db03f2a74865f7b785d.html)

                    *   [Signalprocessing_pal](http://help.scilab.org/docs/5.4.0/ja_JP/Signalprocessing_pal.html) — 信号处理调色板
            *   [QUANT_f](http://help.scilab.org/docs/5.4.0/ja_JP/QUANT_f.html) — 量化
            *   [SAMPHOLD_m](http://help.scilab.org/docs/5.4.0/ja_JP/SAMPHOLD_m.html) — 示例并按住

                *   [Signal routing palette](http://help.scilab.org/docs/5.4.0/ja_JP/section_165653bcb370534d3dc133e98754ad7d.html)

                    *   [Signalrouting_pal](http://help.scilab.org/docs/5.4.0/ja_JP/Signalrouting_pal.html) — 信号路由调色板
            *   [DEMUX](http://help.scilab.org/docs/5.4.0/ja_JP/DEMUX.html) — 解复用器
            *   [EXTRACTOR](http://help.scilab.org/docs/5.4.0/ja_JP/EXTRACTOR.html) — 提取程序
            *   [FROM](http://help.scilab.org/docs/5.4.0/ja_JP/FROM.html) — 从收到数据从相应的跳转到
            *   [FROMMO](http://help.scilab.org/docs/5.4.0/ja_JP/FROMMO.html) — 从相应的 GOTOMO 接收数据
            *   [GOTO](http://help.scilab.org/docs/5.4.0/ja_JP/GOTO.html) — 转到通行证块从块输入到
            *   [GOTOMO](http://help.scilab.org/docs/5.4.0/ja_JP/GOTOMO.html) — 将块输入传递给 FROMMO 块
            *   [GotoTagVisibility](http://help.scilab.org/docs/5.4.0/ja_JP/GotoTagVisibility.html) — 定义跳转到标记可见性的范围
            *   [GotoTagVisibilityMO](http://help.scilab.org/docs/5.4.0/ja_JP/GotoTagVisibilityMO.html) — 定义范围的 GOTOMO 标记可见性
            *   [ISELECT_m](http://help.scilab.org/docs/5.4.0/ja_JP/ISELECT_m.html) — 中选择要导出
            *   [MUX](http://help.scilab.org/docs/5.4.0/ja_JP/MUX.html) — 多路复用器
            *   [M_SWITCH](http://help.scilab.org/docs/5.4.0/ja_JP/M_SWITCH.html) — 多端口的交换机
            *   [NRMSOM_f](http://help.scilab.org/docs/5.4.0/ja_JP/NRMSOM_f.html) — 合并数据
            *   [RELAY_f](http://help.scilab.org/docs/5.4.0/ja_JP/RELAY_f.html) — 中继
            *   [SELECT_m](http://help.scilab.org/docs/5.4.0/ja_JP/SELECT_m.html) — 请选择
            *   [SELF_SWITCH](http://help.scilab.org/docs/5.4.0/ja_JP/SELF_SWITCH.html) — 开关
            *   [SWITCH2_m](http://help.scilab.org/docs/5.4.0/ja_JP/SWITCH2_m.html) — SWITCH2
            *   [SWITCH_f](http://help.scilab.org/docs/5.4.0/ja_JP/SWITCH_f.html) — 开关

                *   [Sinks palette](http://help.scilab.org/docs/5.4.0/ja_JP/section_f99a8754caf17e7a06364db519ab26f0.html)

                    *   [Sinks_pal](http://help.scilab.org/docs/5.4.0/ja_JP/Sinks_pal.html) — 汇调色板
            *   [AFFICH_m](http://help.scilab.org/docs/5.4.0/ja_JP/AFFICH_m.html) — 显示
            *   [BARXY](http://help.scilab.org/docs/5.4.0/ja_JP/BARXY.html) — y = f (x) 动画查看器
            *   [CANIMXY](http://help.scilab.org/docs/5.4.0/ja_JP/CANIMXY.html) — y = f (x) 动画查看器
            *   [CANIMXY3D](http://help.scilab.org/docs/5.4.0/ja_JP/CANIMXY3D.html) — z = f (x，y) 动画查看器
            *   [CFSCOPE](http://help.scilab.org/docs/5.4.0/ja_JP/CFSCOPE.html) — 浮动点范围
            *   [CMAT3D](http://help.scilab.org/docs/5.4.0/ja_JP/CMAT3D.html) — 矩阵 z 值 3D 查看器
            *   [CMATVIEW](http://help.scilab.org/docs/5.4.0/ja_JP/CMATVIEW.html) — 矩阵 Colormapped 查看器
            *   [CMSCOPE](http://help.scilab.org/docs/5.4.0/ja_JP/CMSCOPE.html) — 多显示范围
            *   [CSCOPE](http://help.scilab.org/docs/5.4.0/ja_JP/CSCOPE.html) — 单个显示范围
            *   [CSCOPXY](http://help.scilab.org/docs/5.4.0/ja_JP/CSCOPXY.html) — y = f (x) 永久查看器
            *   [CSCOPXY3D](http://help.scilab.org/docs/5.4.0/ja_JP/CSCOPXY3D.html) — z = f (x，y) 永久查看器
            *   [ENDBLK](http://help.scilab.org/docs/5.4.0/ja_JP/ENDBLK.html) — END 块
            *   [END_c](http://help.scilab.org/docs/5.4.0/ja_JP/END_c.html) — END_c 块
            *   [TOWS_c](http://help.scilab.org/docs/5.4.0/ja_JP/TOWS_c.html) — Scilab worspace 的数据
            *   [TRASH_f](http://help.scilab.org/docs/5.4.0/ja_JP/TRASH_f.html) — 垃圾块
            *   [WFILE_f](http://help.scilab.org/docs/5.4.0/ja_JP/WFILE_f.html) — 写入的输出文件。 此函数已过时。
            *   [WRITEAU_f](http://help.scilab.org/docs/5.4.0/ja_JP/WRITEAU_f.html) — 写非盟声音文件
            *   [WRITEC_f](http://help.scilab.org/docs/5.4.0/ja_JP/WRITEC_f.html) — 写入二进制文件 C

                *   [Sources palette](http://help.scilab.org/docs/5.4.0/ja_JP/section_8a1489921d90780d12f2145184cc7263.html)

                    *   [Sources_pal](http://help.scilab.org/docs/5.4.0/ja_JP/Sources_pal.html) — 源调色板
            *   [CLOCK_c](http://help.scilab.org/docs/5.4.0/ja_JP/CLOCK_c.html) — 激活时钟
            *   [CONST_m](http://help.scilab.org/docs/5.4.0/ja_JP/CONST_m.html) — 常量
            *   [CURV_f](http://help.scilab.org/docs/5.4.0/ja_JP/CURV_f.html) — 曲线
            *   [Counter](http://help.scilab.org/docs/5.4.0/ja_JP/Counter.html) — 计数器
            *   [FROMWSB](http://help.scilab.org/docs/5.4.0/ja_JP/FROMWSB.html) — Scilab 工作区中的数据到 Xcos
            *   [GENSIN_f](http://help.scilab.org/docs/5.4.0/ja_JP/GENSIN_f.html) — 正弦波发生器
            *   [GENSQR_f](http://help.scilab.org/docs/5.4.0/ja_JP/GENSQR_f.html) — 方波发生器
            *   [Modulo_Count](http://help.scilab.org/docs/5.4.0/ja_JP/Modulo_Count.html) — 模计数器 （0 到 N 计数器）
            *   [PULSE_SC](http://help.scilab.org/docs/5.4.0/ja_JP/PULSE_SC.html) — 脉冲发生器
            *   [RAMP](http://help.scilab.org/docs/5.4.0/ja_JP/RAMP.html) — 匝道
            *   [RAND_m](http://help.scilab.org/docs/5.4.0/ja_JP/RAND_m.html) — 随机生成器
            *   [READAU_f](http://help.scilab.org/docs/5.4.0/ja_JP/READAU_f.html) — 读非盟声音文件
            *   [READC_f](http://help.scilab.org/docs/5.4.0/ja_JP/READC_f.html) — 读取二进制数据
            *   [RFILE_f](http://help.scilab.org/docs/5.4.0/ja_JP/RFILE_f.html) — 从输入文件中读取
            *   [SAWTOOTH_f](http://help.scilab.org/docs/5.4.0/ja_JP/SAWTOOTH_f.html) — 锯齿发生器
            *   [STEP_FUNCTION](http://help.scilab.org/docs/5.4.0/ja_JP/STEP_FUNCTION.html) — 阶跃函数
            *   [SampleCLK](http://help.scilab.org/docs/5.4.0/ja_JP/SampleCLK.html) — 示例时间时钟
            *   [Sigbuilder](http://help.scilab.org/docs/5.4.0/ja_JP/Sigbuilder.html) — 发生器创建者
            *   [TIME_f](http://help.scilab.org/docs/5.4.0/ja_JP/TIME_f.html) — 时间
            *   [TKSCALE](http://help.scilab.org/docs/5.4.0/ja_JP/TKSCALE.html) — 调整的值与一个图形化的构件。

                *   [Thermohydraulics palette](http://help.scilab.org/docs/5.4.0/ja_JP/section_1e3a83a9c708612d9301b772577937d5.html)

                    *   [ThermoHydraulics_pal](http://help.scilab.org/docs/5.4.0/ja_JP/ThermoHydraulics_pal.html) — 热工水力学工具箱
            *   [Bache](http://help.scilab.org/docs/5.4.0/ja_JP/Bache.html) — 热工水力罐 (水库)
            *   [PerteDP](http://help.scilab.org/docs/5.4.0/ja_JP/PerteDP.html) — 热工水力管道
            *   [PuitsP](http://help.scilab.org/docs/5.4.0/ja_JP/PuitsP.html) — (井) 的热工水力流失
            *   [SourceP](http://help.scilab.org/docs/5.4.0/ja_JP/SourceP.html) — 热工水力恒压源
            *   [VanneReglante](http://help.scilab.org/docs/5.4.0/ja_JP/VanneReglante.html) — 热工水力控制阀门

                *   [User defined functions palette](http://help.scilab.org/docs/5.4.0/ja_JP/section_ad1c35e1fbb71486c56dc34d227a0019.html)

                    *   [Userdefinedfunctions_pal](http://help.scilab.org/docs/5.4.0/ja_JP/Userdefinedfunctions_pal.html) — 用户定义的函数调色板
            *   [CBLOCK](http://help.scilab.org/docs/5.4.0/ja_JP/CBLOCK.html) — 新 C
            *   [DSUPER](http://help.scilab.org/docs/5.4.0/ja_JP/DSUPER.html) — 蒙面的超级块
            *   [EXPRESSION](http://help.scilab.org/docs/5.4.0/ja_JP/EXPRESSION.html) — 数学表达式
            *   [MBLOCK](http://help.scilab.org/docs/5.4.0/ja_JP/MBLOCK.html) — Modelica 通用块
            *   [SUPER_f](http://help.scilab.org/docs/5.4.0/ja_JP/SUPER_f.html) — 超级块
            *   [c_block](http://help.scilab.org/docs/5.4.0/ja_JP/c_block.html) — C 语言
            *   [fortran_block](http://help.scilab.org/docs/5.4.0/ja_JP/fortran_block.html) — Fortran
            *   [generic_block3](http://help.scilab.org/docs/5.4.0/ja_JP/generic_block3.html) — 通用块
            *   [scifunc_block_m](http://help.scilab.org/docs/5.4.0/ja_JP/scifunc_block_m.html) — Scilab 功能块

                *   [Zero crossing detection palette](http://help.scilab.org/docs/5.4.0/ja_JP/section_7ad0d9790438217a37d7d6bd3efadbd1.html)

                    *   [Zerocrossingdetection_pal](http://help.scilab.org/docs/5.4.0/ja_JP/Zerocrossingdetection_pal.html) — 零交叉检测调色板
            *   [GENERAL_f](http://help.scilab.org/docs/5.4.0/ja_JP/GENERAL_f.html) — GENERAL_f 标题
            *   [NEGTOPOS_f](http://help.scilab.org/docs/5.4.0/ja_JP/NEGTOPOS_f.html) — 阈值消极到积极
            *   [POSTONEG_f](http://help.scilab.org/docs/5.4.0/ja_JP/POSTONEG_f.html) — 积极到消极的阈值
            *   [ZCROSS_f](http://help.scilab.org/docs/5.4.0/ja_JP/ZCROSS_f.html) — 在零的阈值检测

        *   [Programming xcos Blocks](http://help.scilab.org/docs/5.4.0/ja_JP/section_bd364c0bace36a9235956650016c8bde.html)

            *   [C Computational Functions](http://help.scilab.org/docs/5.4.0/ja_JP/section_253c89741c7f7bdbf176167747a6dbcd.html)

                    *   [C_macros](http://help.scilab.org/docs/5.4.0/ja_JP/C_macros.html) — 实用程序 C 宏
            *   [C_struct](http://help.scilab.org/docs/5.4.0/ja_JP/C_struct.html) — C 块计算函数的结构
            *   [C_utils](http://help.scilab.org/docs/5.4.0/ja_JP/C_utils.html) — 实用程序 C 函数

                *   [Scilab Computational Functions](http://help.scilab.org/docs/5.4.0/ja_JP/section_7fc9eae9f096b05516b88dd02112c1d2.html)

                    *   [sci_struct](http://help.scilab.org/docs/5.4.0/ja_JP/sci_struct.html) — Scicos scilab 计算函数的块结构

                *   [Utilities Functions](http://help.scilab.org/docs/5.4.0/ja_JP/section_6f6a29e0017e54eaef5765cf4c986d9e.html)

                    *   [curblock](http://help.scilab.org/docs/5.4.0/ja_JP/curblock.html) — 在模拟期间返回当前调用的 xcos 块
            *   [getblocklabel](http://help.scilab.org/docs/5.4.0/ja_JP/getblocklabel.html) — 获取 scicos 块的标签
            *   [getscicosvars](http://help.scilab.org/docs/5.4.0/ja_JP/getscicosvars.html) — 主管效用函数
            *   [phase_simulation](http://help.scilab.org/docs/5.4.0/ja_JP/phase_simulation.html) — 获取当前的仿真阶段
            *   [pointer_xproperty](http://help.scilab.org/docs/5.4.0/ja_JP/pointer_xproperty.html) — 获取的连续时间状态变量的类型
            *   [scicos_time](http://help.scilab.org/docs/5.4.0/ja_JP/scicos_time.html) — 返回当前时间期间模拟
            *   [set_blockerror](http://help.scilab.org/docs/5.4.0/ja_JP/set_blockerror.html) — 设置的块错误编号
            *   [set_xproperty](http://help.scilab.org/docs/5.4.0/ja_JP/set_xproperty.html) — 设置连续时间状态变量的类型

        *   [Scilab Utilities Functions](http://help.scilab.org/docs/5.4.0/ja_JP/section_4eee77adf6e8b6ac31835ff64402e9a6.html)

            *   [block_parameter_error](http://help.scilab.org/docs/5.4.0/ja_JP/block_parameter_error.html) — 显示参数的输入的错误的框 Xcos 块
        *   [buildouttb](http://help.scilab.org/docs/5.4.0/ja_JP/buildouttb.html) — 该生成的子列表 %cpr.state.outtb
        *   [create_palette](http://help.scilab.org/docs/5.4.0/ja_JP/create_palette.html) — 调色板发电机
        *   [getModelicaPath](http://help.scilab.org/docs/5.4.0/ja_JP/getModelicaPath.html) — 获取所需的 Xcos 图包含 Modelica 块的 Modelica 目录路径
        *   [get_scicos_version](http://help.scilab.org/docs/5.4.0/ja_JP/get_scicos_version.html) — 获取当前 Scicos 版本
        *   [importXcosDiagram](http://help.scilab.org/docs/5.4.0/ja_JP/importXcosDiagram.html) — 导入上 Scilab Xcos 图
        *   [loadScicos](http://help.scilab.org/docs/5.4.0/ja_JP/loadScicos.html) — 加载 Xcos 模拟本机库。
        *   [loadXcosLibs](http://help.scilab.org/docs/5.4.0/ja_JP/loadXcosLibs.html) — 加载大多数 Xcos 宏
        *   [scicos_debug](http://help.scilab.org/docs/5.4.0/ja_JP/scicos_debug.html) — 设置的 Scicos 调试级别
        *   [scicos_getvalue](http://help.scilab.org/docs/5.4.0/ja_JP/scicos_getvalue.html) — Xcos Xwindow 的对话框
        *   [standard_inputs](http://help.scilab.org/docs/5.4.0/ja_JP/standard_inputs.html) — 获得 Xcos 编辑器中的块的输入端口的位置。
        *   [standard_origin](http://help.scilab.org/docs/5.4.0/ja_JP/standard_origin.html) — 获得一个块 Xcos 编辑器中的位置。
        *   [standard_outputs](http://help.scilab.org/docs/5.4.0/ja_JP/standard_outputs.html) — 获得一个块的输出端口 Xcos 编辑器中的位置。
        *   [var2vec](http://help.scilab.org/docs/5.4.0/ja_JP/var2vec.html) — 变换 scilab 变量的双重向量中
        *   [vec2var](http://help.scilab.org/docs/5.4.0/ja_JP/vec2var.html) — 变换的向量的双 scilab 变量中
        *   [xcosPal](http://help.scilab.org/docs/5.4.0/ja_JP/xcosPal.html) — Instanciate 对 Scilab 新 Xcos 调色板。
        *   [xcosPalAdd](http://help.scilab.org/docs/5.4.0/ja_JP/xcosPalAdd.html) — 将调色板添加到 Scilab/Xcos 面板管理器。 调色板中的和类别，在添加设置，可选属性即可。
        *   [xcosPalAddBlock](http://help.scilab.org/docs/5.4.0/ja_JP/xcosPalAddBlock.html) — 例如，将块添加成 Scilab/Xcos 的调色板。 可以将一些可选属性添加自定义的调色板图标和块的样式。
        *   [xcosPalExport](http://help.scilab.org/docs/5.4.0/ja_JP/xcosPalExport.html) — 将调色板实例导出到路径。

        *   [xcos](http://help.scilab.org/docs/5.4.0/ja_JP/xcos.html) — GUI 和模拟器的块图编辑器
    *   [xcos_menu_entries](http://help.scilab.org/docs/5.4.0/ja_JP/xcos_menu_entries.html) — 编辑器中的菜单项

*   电子表格[Spreadsheet](http://help.scilab.org/docs/5.4.0/ja_JP/section_5a24fc6ca41cf8a3e9651236d2ec8673.html)

    *   [csvDefault](http://help.scilab.org/docs/5.4.0/ja_JP/csvDefault.html) — 获取/设置为 CSV 文件的默认行为。
    *   [csvRead](http://help.scilab.org/docs/5.4.0/ja_JP/csvRead.html) — CSV 文件加载
    *   [csvTextScan](http://help.scilab.org/docs/5.4.0/ja_JP/csvTextScan.html) — 将用逗号分隔的值矩阵转换
    *   [csvWrite](http://help.scilab.org/docs/5.4.0/ja_JP/csvWrite.html) — 写入 CSV 文件
    *   [read_csv](http://help.scilab.org/docs/5.4.0/ja_JP/read_csv.html) — 导入逗号分隔值文件
    *   [readxls](http://help.scilab.org/docs/5.4.0/ja_JP/readxls.html) — 加载 Excel 文件
    *   [write_csv](http://help.scilab.org/docs/5.4.0/ja_JP/write_csv.html) — 以逗号分隔格式写入文件
    *   [xls_open](http://help.scilab.org/docs/5.4.0/ja_JP/xls_open.html) — 打开 Excel 文件进行读取
    *   [xls_read](http://help.scilab.org/docs/5.4.0/ja_JP/xls_read.html) — 从 Excel 文件中加载表

*   控制台[Console](http://help.scilab.org/docs/5.4.0/ja_JP/section_b80fbe0b8ae7782d30bd0b271b118c4e.html)

    *   [clc](http://help.scilab.org/docs/5.4.0/ja_JP/clc.html) — 清除命令窗口
    *   [completion](http://help.scilab.org/docs/5.4.0/ja_JP/completion.html) — 返回作为参数指定的文本的开头的单词。
    *   [console](http://help.scilab.org/docs/5.4.0/ja_JP/console.html) — 在控制台窗口键盘快捷方式
    *   [diary](http://help.scilab.org/docs/5.4.0/ja_JP/diary.html) — 会话的日记
    *   [lines](http://help.scilab.org/docs/5.4.0/ja_JP/lines.html) — 用于显示行和列
    *   [prompt](http://help.scilab.org/docs/5.4.0/ja_JP/prompt.html) — 获取/设置当前提示
    *   [tohome](http://help.scilab.org/docs/5.4.0/ja_JP/tohome.html) — 将光标移动到左上角的主机名

*   历史管理[History manager](http://help.scilab.org/docs/5.4.0/ja_JP/section_0bfa575d038115c559464009371036dd.html)

    *   [addhistory](http://help.scilab.org/docs/5.4.0/ja_JP/addhistory.html) — 若要添加到当前的堆栈。
    *   [browsehistory](http://help.scilab.org/docs/5.4.0/ja_JP/browsehistory.html) — 打开 Scilab 历史记录浏览器
    *   [displayhistory](http://help.scilab.org/docs/5.4.0/ja_JP/displayhistory.html) — 查看 Scilab 历史记录
    *   [gethistory](http://help.scilab.org/docs/5.4.0/ja_JP/gethistory.html) — 获取一个字符串矩阵 Scilab 历史
    *   [gethistoryfile](http://help.scilab.org/docs/5.4.0/ja_JP/gethistoryfile.html) — 获取用于 Scilab 历史的文件的名称
    *   [historymanager](http://help.scilab.org/docs/5.4.0/ja_JP/historymanager.html) — 若要启用 / 禁用历史记录管理器
    *   [historysize](http://help.scilab.org/docs/5.4.0/ja_JP/historysize.html) — 获取历史记录行的数
    *   [loadhistory](http://help.scilab.org/docs/5.4.0/ja_JP/loadhistory.html) — 历史文件加载
    *   [removelinehistory](http://help.scilab.org/docs/5.4.0/ja_JP/removelinehistory.html) — 删除 N 行的历史记录。
    *   [resethistory](http://help.scilab.org/docs/5.4.0/ja_JP/resethistory.html) — 若要删除 Scilab 历史记录中的所有条目。
    *   [saveafterncommands](http://help.scilab.org/docs/5.4.0/ja_JP/saveafterncommands.html) — 后添加 n 命令，要保存的文件的历史记录文件。
    *   [saveconsecutivecommands](http://help.scilab.org/docs/5.4.0/ja_JP/saveconsecutivecommands.html) — 存储冗余的命令序列。
    *   [savehistory](http://help.scilab.org/docs/5.4.0/ja_JP/savehistory.html) — 将历史记录保存到文件
    *   [sethistoryfile](http://help.scilab.org/docs/5.4.0/ja_JP/sethistoryfile.html) — 设置的文件名 Scilab 历史

*   Matlab二进制文件IO[Matlab binary files I/O](http://help.scilab.org/docs/5.4.0/ja_JP/section_5f5577c7a3ea5f90a7c129ab98efcee5.html)

    *   [loadmatfile](http://help.scilab.org/docs/5.4.0/ja_JP/loadmatfile.html) — lMatlab V6 垫文件加载 （二进制或 ASCII) 到 Scilab
    *   [matfile_close](http://help.scilab.org/docs/5.4.0/ja_JP/matfile_close.html) — Matlab V5 二进制垫文件关闭。
    *   [matfile_listvar](http://help.scilab.org/docs/5.4.0/ja_JP/matfile_listvar.html) — Matlab V5 二进制垫文件中获取的变量的列表。
    *   [matfile_open](http://help.scilab.org/docs/5.4.0/ja_JP/matfile_open.html) — 打开一个 Matlab V5 二进制垫文件。
    *   [matfile_varreadnext](http://help.scilab.org/docs/5.4.0/ja_JP/matfile_varreadnext.html) — 加载一个 Matlab V5 二进制垫文件中的变量。
    *   [matfile_varwrite](http://help.scilab.org/docs/5.4.0/ja_JP/matfile_varwrite.html) — 写变量 Matlab V5 二进制垫-文件。
    *   [savematfile](http://help.scilab.org/docs/5.4.0/ja_JP/savematfile.html) — 编写一个 Matlab 垫文件 （二进制或 ASCII)

*   [Matlab to Scilab Conversion Tips](http://help.scilab.org/docs/5.4.0/ja_JP/section_ae2592d894269512e285ea09e899bcb4.html)

    *   [Matlab-Scilab equivalents](http://help.scilab.org/docs/5.4.0/ja_JP/section_36184e52ee88ad558380be4e92d3de21.html)

            *   [A](http://help.scilab.org/docs/5.4.0/ja_JP/section_113ebab21f66f9f97431801ec314fe5a.html)

                    *   [m2sci_abs](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_abs.html) — 绝对价值和复杂程度
            *   [m2sci_acos](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_acos.html) — 反余弦值
            *   [m2sci_acosh](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_acosh.html) — 反双曲余弦值
            *   [m2sci_acot](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_acot.html) — 反余切
            *   [m2sci_acoth](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_acoth.html) — 反双曲余切
            *   [m2sci_acsc](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_acsc.html) — 反余割
            *   [m2sci_acsch](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_acsch.html) — 反双曲余割
            *   [m2sci_all](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_all.html) — 测试以确定是否所有元素非零
            *   [m2sci_angle](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_angle.html) — 相角
            *   [m2sci_any](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_any.html) — 测试以确定是否有任何 nonzeros 的元素
            *   [m2sci_asec](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_asec.html) — 反正割
            *   [m2sci_asech](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_asech.html) — 反双曲正割
            *   [m2sci_asin](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_asin.html) — 反正弦值
            *   [m2sci_asinh](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_asinh.html) — 反双曲正弦值
            *   [m2sci_atan](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_atan.html) — 两象限反正切值
            *   [m2sci_atan2](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_atan2.html) — 四象限反正切值
            *   [m2sci_atanh](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_atanh.html) — 反双曲正切值

                *   [B](http://help.scilab.org/docs/5.4.0/ja_JP/section_7c1907e9d96f63d76690134bb2e99d6f.html)

                    *   [m2sci_balance](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_balance.html) — 扩展以改善特征值准确性的对角线
            *   [m2sci_bar](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_bar.html) — 条形直方图
            *   [m2sci_barh](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_barh.html) — 直方图水平栏
            *   [m2sci_beep](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_beep.html) — 产生蜂鸣声
            *   [m2sci_besseli](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_besseli.html) — 第一种改性的贝塞尔函数
            *   [m2sci_besselj](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_besselj.html) — 第一类贝塞尔函数
            *   [m2sci_besselk](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_besselk.html) — 第二类改性的贝塞尔函数
            *   [m2sci_bessely](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_bessely.html) — 第二类贝塞尔函数
            *   [m2sci_beta](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_beta.html) — Beta 函数
            *   [m2sci_bin2dec](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_bin2dec.html) — 返回对应于给定的二进制表示形式的整数
            *   [m2sci_bitand](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_bitand.html) — 与两个整数的
            *   [m2sci_bitcmp](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_bitcmp.html) — 补充一个整数的二进制文件
            *   [m2sci_bitget](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_bitget.html) — 获取一个整数，其当前位置鉴于在输入参数中的位
            *   [m2sci_bitor](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_bitor.html) — 两个整数同或
            *   [m2sci_bitxor](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_bitxor.html) — 返回两个整数的独占或
            *   [m2sci_blanks](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_blanks.html) — 一个空格的字符串
            *   [m2sci_box](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_box.html) — 显示轴边框
            *   [m2sci_break](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_break.html) — 终止执行 for 循环或 while 循环

                *   [C](http://help.scilab.org/docs/5.4.0/ja_JP/section_16cbd0754127f7ce3b7c82c45d0a25e3.html)

                    *   [m2sci_case](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_case.html) — 切换大小写
            *   [m2sci_cat](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_cat.html) — 阵列串联
            *   [m2sci_cd](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_cd.html) — 更改/获取工作目录
            *   [m2sci_ceil](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_ceil.html) — 向上舍入
            *   [m2sci_cell](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_cell.html) — 创建单元格的数组
            *   [m2sci_cell2mat](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_cell2mat.html) — 将一个单元格数组转换成一个矩阵
            *   [m2sci_cellstr](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_cellstr.html) — 将字符串向量 （或字符串矩阵） 转换成字符串的单元格
            *   [m2sci_chol](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_chol.html) — 乔莱斯基分解
            *   [m2sci_cla](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_cla.html) — 清除当前轴
            *   [m2sci_clc](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_clc.html) — 明确的命令窗口
            *   [m2sci_clear](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_clear.html) — 从工作区中，释放系统内存中删除项目
            *   [m2sci_clf](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_clf.html) — 清除当前图窗口
            *   [m2sci_clock](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_clock.html) — 作为一个日期向量的当前时间
            *   [m2sci_close](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_close.html) — 删除指定的图
            *   [m2sci_closereq](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_closereq.html) — 默认图关闭请求函数
            *   [m2sci_colordef](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_colordef.html) — 设置默认的属性值，以显示不同的配色方案
            *   [m2sci_complex](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_complex.html) — 返回对应于给定的实部和虚部的一部分的复杂形式
            *   [m2sci_conj](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_conj.html) — 共轭复数
            *   [m2sci_continue](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_continue.html) — 关键字将控制传递到循环的下一个迭代
            *   [m2sci_conv](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_conv.html) — 1-D 卷积
            *   [m2sci_conv2](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_conv2.html) — 2-D 卷积
            *   [m2sci_cos](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_cos.html) — 余弦
            *   [m2sci_cosh](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_cosh.html) — 双曲余弦值
            *   [m2sci_cot](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_cot.html) — 余切
            *   [m2sci_coth](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_coth.html) — 双曲余切
            *   [m2sci_cputime](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_cputime.html) — 已用的 CPU 时间
            *   [m2sci_csc](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_csc.html) — 余割
            *   [m2sci_csch](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_csch.html) — 双曲余割
            *   [m2sci_cumprod](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_cumprod.html) — 累积产品
            *   [m2sci_cumsum](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_cumsum.html) — 累积总和

                *   [D](http://help.scilab.org/docs/5.4.0/ja_JP/section_e221baa74add8444775cb6687a29b2f7.html)

                    *   [m2sci_date](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_date.html) — 当前日期的字符串
            *   [m2sci_dec2bin](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_dec2bin.html) — 十进制数的二进制表示形式
            *   [m2sci_dec2hex](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_dec2hex.html) — 十六进制数转换为十进制
            *   [m2sci_delete](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_delete.html) — 删除文件或图形对象
            *   [m2sci_det](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_det.html) — 行列式
            *   [m2sci_diag](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_diag.html) — 对角线包括或提取
            *   [m2sci_diary](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_diary.html) — 将会话保存到一个文件
            *   [m2sci_diff](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_diff.html) — 差异和近似衍生品
            *   [m2sci_dir](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_dir.html) — 显示目录列表
            *   [m2sci_disp](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_disp.html) — 显示文本或数组
            *   [m2sci_display](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_display.html) — 重载的方法，以显示对象
            *   [m2sci_doc](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_doc.html) — 显示联机文档
            *   [m2sci_docopt](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_docopt.html) — 对于 UNIX 平台的 web 浏览器
            *   [m2sci_dos](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_dos.html) — 执行 UNIX 命令并返回结果
            *   [m2sci_double](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_double.html) — 转换为双精度
            *   [m2sci_drawnow](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_drawnow.html) — 挂起的绘制事件完成

                *   [E](http://help.scilab.org/docs/5.4.0/ja_JP/section_68f9e858e116a06824d3688eced22705.html)

                    *   [m2sci_echo](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_echo.html) — 在执行过程中的回波行
            *   [m2sci_eig](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_eig.html) — 找到特征值和特征向量
            *   [m2sci_else](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_else.html) — 有条件地执行语句
            *   [m2sci_elseif](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_elseif.html) — 有条件地执行语句
            *   [m2sci_erf](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_erf.html) — 误差函数
            *   [m2sci_erfc](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_erfc.html) — 互补误差函数
            *   [m2sci_erfcx](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_erfcx.html) — 缩放互补错误函数
            *   [m2sci_error](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_error.html) — 显示的错误消息
            *   [m2sci_etime](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_etime.html) — 经过的时间
            *   [m2sci_eval](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_eval.html) — 执行一个字符串，包含指令/表达式
            *   [m2sci_exist](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_exist.html) — 检查是否存在变量或文件
            *   [m2sci_exit](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_exit.html) — 结束当前会话
            *   [m2sci_exp](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_exp.html) — 指数
            *   [m2sci_expm](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_expm.html) — 矩阵指数
            *   [m2sci_eye](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_eye.html) — 恒等矩阵

                *   [F](http://help.scilab.org/docs/5.4.0/ja_JP/section_9c44ee6dead777df36ace153190f38df.html)

                    *   [m2sci_factor](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_factor.html) — 素数分解
            *   [m2sci_false](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_false.html) — 虚假的数组
            *   [m2sci_fclose](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_fclose.html) — 关闭一个或多个打开的文件
            *   [m2sci_feof](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_feof.html) — 测试的文件结束
            *   [m2sci_ferror](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_ferror.html) — 查询有关文件输入或输出中的错误
            *   [m2sci_feval](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_feval.html) — 函数求值
            *   [m2sci_fft](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_fft.html) — 离散傅里叶变换
            *   [m2sci_fftshift](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_fftshift.html) — Shift 频率为零组件的离散傅里叶变换光谱的中心
            *   [m2sci_fgetl](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_fgetl.html) — (S) 从文件中读取行，丢弃换行符
            *   [m2sci_fgets](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_fgets.html) — 从文件中读取行，保留换行符
            *   [m2sci_fileparts](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_fileparts.html) — 返回文件名部分
            *   [m2sci_filesep](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_filesep.html) — 返回此平台的目录分隔符
            *   [m2sci_find](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_find.html) — 找到的指数和非零元素的值
            *   [m2sci_findstr](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_findstr.html) — 查找一个字符串在另一个字符串
            *   [m2sci_fix](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_fix.html) — 向零方向
            *   [m2sci_fliplr](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_fliplr.html) — 左/右方向翻转矩阵
            *   [m2sci_flipud](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_flipud.html) — 向上/向下方向翻转矩阵
            *   [m2sci_floor](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_floor.html) — 向下舍入
            *   [m2sci_fopen](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_fopen.html) — 打开一个文件或获取有关打开的文件的信息
            *   [m2sci_for](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_for.html) — 重复特定次数的语句
            *   [m2sci_format](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_format.html) — 控制显示格式的输出
            *   [m2sci_fprintf](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_fprintf.html) — 带格式的数据写入文件
            *   [m2sci_fread](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_fread.html) — 读取二进制数据到文件
            *   [m2sci_frewind](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_frewind.html) — 将文件位置指示器移动到打开的文件的开头
            *   [m2sci_fscanf](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_fscanf.html) — 读取格式的数据文件
            *   [m2sci_fseek](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_fseek.html) — 设置文件位置指示器
            *   [m2sci_ftell](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_ftell.html) — 获取文件位置指示器
            *   [m2sci_full](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_full.html) — 将稀疏矩阵转换到全矩阵
            *   [m2sci_fullfile](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_fullfile.html) — 生成完整的文件名，从部件
            *   [m2sci_function](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_function.html) — 函数定义
            *   [m2sci_fwrite](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_fwrite.html) — 向文件中写入二进制数据

                *   [G](http://help.scilab.org/docs/5.4.0/ja_JP/section_d1bba7cc09d5622725cee5bf342f1389.html)

                    *   [m2sci_gamma](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_gamma.html) — 伽玛函数
            *   [m2sci_gammaln](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_gammaln.html) — 伽玛函数的对数
            *   [m2sci_getenv](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_getenv.html) — 获取环境变量
            *   [m2sci_global](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_global.html) — 定义一个全局变量
            *   [m2sci_graymon](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_graymon.html) — 灰阶显示器设置的图形的默认值
            *   [m2sci_grid](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_grid.html) — 两个网格线-和三维地块

                *   [H](http://help.scilab.org/docs/5.4.0/ja_JP/section_cc461ac53f844d1a98b79bbce1d6e0e9.html)

                    *   [m2sci_hankel](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_hankel.html) — 汉克尔矩阵
            *   [m2sci_help](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_help.html) — 显示帮助
            *   [m2sci_helpbrowser](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_helpbrowser.html) — 显示帮助浏览器访问完整联机文档
            *   [m2sci_helpdesk](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_helpdesk.html) — 显示帮助浏览器
            *   [m2sci_helpwin](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_helpwin.html) — 提供访问和显示所有函数的帮助
            *   [m2sci_hess](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_hess.html) — Hessenberg 形式的矩阵
            *   [m2sci_hold](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_hold.html) — 保存当前关系图
            *   [m2sci_home](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_home.html) — 将光标移动到左上角的命令窗口
            *   [m2sci_horzcat](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_horzcat.html) — 水平串联

                *   [I](http://help.scilab.org/docs/5.4.0/ja_JP/section_97b060d7308d5842e9aaa7eebafe1be5.html)

                    *   [m2sci_if](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_if.html) — 有条件地执行语句
            *   [m2sci_ifft](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_ifft.html) — 逆离散傅立叶变换
            *   [m2sci_imag](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_imag.html) — 复杂的虚数部分
            *   [m2sci_input](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_input.html) — 要求用户输入
            *   [m2sci_int16](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_int16.html) — 将转换为 16 位带符号整数
            *   [m2sci_int32](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_int32.html) — 将转换为 32 位有符号整数
            *   [m2sci_int8](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_int8.html) — 将转换为 8 位带符号整数
            *   [m2sci_interp1](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_interp1.html) — One_dimension 插值函数
            *   [m2sci_inv](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_inv.html) — 矩阵逆
            *   [m2sci_isa](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_isa.html) — 检测到一个给定类型的对象
            *   [m2sci_iscell](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_iscell.html) — 确定输入是否为一个单元格数组
            *   [m2sci_ischar](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_ischar.html) — 确定是否该项目是一个字符数组
            *   [m2sci_isdir](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_isdir.html) — 确定该项目是否为目录
            *   [m2sci_isempty](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_isempty.html) — 为 true，空矩阵
            *   [m2sci_isequal](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_isequal.html) — 确定数组是否数值相等
            *   [m2sci_isfield](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_isfield.html) — 确定输入是否是一个结构数组字段
            *   [m2sci_isfinite](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_isfinite.html) — 有限元素为 true
            *   [m2sci_isglobal](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_isglobal.html) — 确定是否该项目是一个全局变量
            *   [m2sci_ishandle](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_ishandle.html) — 确定值是否有效图形对象句柄
            *   [m2sci_ishold](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_ishold.html) — 返回保持状态
            *   [m2sci_isinf](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_isinf.html) — 真正的无限元素
            *   [m2sci_isinteger](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_isinteger.html) — 检测数组是否具有整数数据类型
            *   [m2sci_isletter](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_isletter.html) — 为 true，字母表的字母
            *   [m2sci_islogical](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_islogical.html) — 确定该项目是否逻辑阵列
            *   [m2sci_isnan](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_isnan.html) — 检测南一个数组的元素
            *   [m2sci_isnumeric](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_isnumeric.html) — 确定输入是否数值数组
            *   [m2sci_ispc](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_ispc.html) — 确定如果 PC （Windows） 版本
            *   [m2sci_isreal](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_isreal.html) — 确定是否所有数组元素都是实数
            *   [m2sci_isscalar](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_isscalar.html) — 确定输入是否为标量
            *   [m2sci_isspace](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_isspace.html) — 检测 ASCII 空格的元素
            *   [m2sci_issparse](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_issparse.html) — 如果矩阵是稀疏的测试
            *   [m2sci_isstr](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_isstr.html) — 确定是否该项目是一个字符数组
            *   [m2sci_isstruct](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_isstruct.html) — 确定输入是否是一个结构数组
            *   [m2sci_isunix](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_isunix.html) — 确定如果 Unix 版本
            *   [m2sci_isvector](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_isvector.html) — 确定是否输入是一个矢量

                *   [K](http://help.scilab.org/docs/5.4.0/ja_JP/section_871fb6ddb1ce293af320ea15057e2ae5.html)

                    *   [m2sci_keyboard](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_keyboard.html) — 调用文件中的键盘
            *   [m2sci_kron](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_kron.html) — 张量积

                *   [L](http://help.scilab.org/docs/5.4.0/ja_JP/section_d4660190e220fc095b542dee112c9ade.html)

                    *   [m2sci_length](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_length.html) — 向量的长度
            *   [m2sci_linspace](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_linspace.html) — 线性间隔的矢量
            *   [m2sci_load](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_load.html) — 从磁盘加载工作区变量
            *   [m2sci_log](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_log.html) — 自然对数
            *   [m2sci_log10](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_log10.html) — （基数 10） 常用对数
            *   [m2sci_log2](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_log2.html) — 基地 2 对数和解剖浮点数
            *   [m2sci_logical](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_logical.html) — 将数值转换为逻辑
            *   [m2sci_lookfor](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_lookfor.html) — 在所有的帮助中搜索指定的关键字的条目
            *   [m2sci_lower](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_lower.html) — 将字符串转换为小写
            *   [m2sci_lu](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_lu.html) — LU 矩阵分解

                *   [M](http://help.scilab.org/docs/5.4.0/ja_JP/section_b33dc7db7b62cf0fd509dcac5d44ef81.html)

                    *   [m2sci_max](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_max.html) — 最大值
            *   [m2sci_min](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_min.html) — 最低
            *   [m2sci_mkdir](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_mkdir.html) — 创建一个新文件夹
            *   [m2sci_mod](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_mod.html) — 分立后的模数
            *   [m2sci_more](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_more.html) — 一次显示命令窗口输出一个满屏

                *   [N](http://help.scilab.org/docs/5.4.0/ja_JP/section_2933224185593aade2187c8140e8bf45.html)

                    *   [m2sci_nargin](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_nargin.html) — 函数的输入参数的数目
            *   [m2sci_nargout](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_nargout.html) — 函数输出参数的数目
            *   [m2sci_ndims](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_ndims.html) — 数组的维数
            *   [m2sci_norm](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_norm.html) — 向量和矩阵的规范
            *   [m2sci_num2str](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_num2str.html) — 字符串转换为数字

                *   [O](http://help.scilab.org/docs/5.4.0/ja_JP/section_cf12333967f2868ef0ba17cc0c81059b.html)

                    *   [m2sci_ones](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_ones.html) — 创建一个数组的所有
            *   [m2sci_otherwise](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_otherwise.html) — 默认开关/选择语句的一部分
            *   [m2sci_pause](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_pause.html) — 暂时停止执行

                *   [Operators](http://help.scilab.org/docs/5.4.0/ja_JP/section_dd5a9aee4c50bc4024410646f60d4aa3.html)

                    *   [m2sci_addition](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_addition.html) — 加号
            *   [m2sci_and](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_and.html) — 逻辑和
            *   [m2sci_colon](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_colon.html) — 冒号
            *   [m2sci_elementwise_left_division](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_elementwise_left_division.html) — Elementwise 左司
            *   [m2sci_elementwise_multiplication](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_elementwise_multiplication.html) — Elementwise 乘法
            *   [m2sci_elementwise_power](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_elementwise_power.html) — Elementwise 指数
            *   [m2sci_elementwise_right_division](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_elementwise_right_division.html) — Elementwise 右司
            *   [m2sci_elementwise_transpose](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_elementwise_transpose.html) — Elementwise 转置
            *   [m2sci_equal](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_equal.html) — 等于
            *   [m2sci_great](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_great.html) — 大于
            *   [m2sci_great_equal](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_great_equal.html) — 大于或等于
            *   [m2sci_left_division](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_left_division.html) — 左的司
            *   [m2sci_less](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_less.html) — 比小
            *   [m2sci_less_equal](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_less_equal.html) — 小于或等于
            *   [m2sci_multiplication](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_multiplication.html) — 乘法
            *   [m2sci_not](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_not.html) — 否定
            *   [m2sci_not_equal](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_not_equal.html) — 不等于
            *   [m2sci_or](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_or.html) — 逻辑或
            *   [m2sci_power](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_power.html) — 指数
            *   [m2sci_right_division](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_right_division.html) — 右司
            *   [m2sci_substraction](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_substraction.html) — 减号
            *   [m2sci_transpose](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_transpose.html) — 转置

                *   [P](http://help.scilab.org/docs/5.4.0/ja_JP/section_abd21efc9b48b6b366603f6e58456e57.html)

                    *   [m2sci_perms](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_perms.html) — 向量组件的所有排列的数组
            *   [m2sci_permute](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_permute.html) — Permute 数组的维数
            *   [m2sci_pie](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_pie.html) — 圆形图形
            *   [m2sci_plot](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_plot.html) — 线性 2-d 地块
            *   [m2sci_pow2](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_pow2.html) — 基地 2 电源和规模的浮点数
            *   [m2sci_primes](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_primes.html) — 返回包括 1 之间，鉴于数目的素数数字
            *   [m2sci_prod](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_prod.html) — 数组元素的乘积

                *   [Q](http://help.scilab.org/docs/5.4.0/ja_JP/section_4eb803b1257dcfab1d1253fef3552170.html)

                    *   [m2sci_qr](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_qr.html) — 正交三角分解
            *   [m2sci_quit](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_quit.html) — 终止会话

                *   [R](http://help.scilab.org/docs/5.4.0/ja_JP/section_e871a0fa7f0df41bc1beb41aa9a47fe1.html)

                    *   [m2sci_rand](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_rand.html) — 均匀分布随机数和阵列
            *   [m2sci_randn](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_randn.html) — 通常分布随机数和阵列
            *   [m2sci_rcond](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_rcond.html) — 矩阵对应的条件数估计
            *   [m2sci_real](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_real.html) — 复数的实数部分
            *   [m2sci_realmax](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_realmax.html) — 最积极的浮点数
            *   [m2sci_realmin](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_realmin.html) — 最小的正数浮点
            *   [m2sci_rem](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_rem.html) — 分立后的余数
            *   [m2sci_repmat](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_repmat.html) — 复制并平铺数组
            *   [m2sci_reshape](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_reshape.html) — 重塑数组
            *   [m2sci_return](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_return.html) — 返回到调用函数
            *   [m2sci_round](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_round.html) — 舍入到最接近的整数

                *   [S](http://help.scilab.org/docs/5.4.0/ja_JP/section_f2afb3612395ff0898ebdbee36a1652b.html)

                    *   [m2sci_save](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_save.html) — 从磁盘中保存工作区变量
            *   [m2sci_schur](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_schur.html) — Schur 分解
            *   [m2sci_setstr](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_setstr.html) — 设置字符串标志
            *   [m2sci_sign](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_sign.html) — Signum 函数
            *   [m2sci_sin](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_sin.html) — 正弦
            *   [m2sci_sinh](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_sinh.html) — 双曲正弦值
            *   [m2sci_size](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_size.html) — 数组维度
            *   [m2sci_sort](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_sort.html) — 在按升序对元素进行排序
            *   [m2sci_sparse](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_sparse.html) — 创建稀疏矩阵
            *   [m2sci_sqrt](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_sqrt.html) — 平方根
            *   [m2sci_strcmp](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_strcmp.html) — 比较字符串
            *   [m2sci_strcmpi](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_strcmpi.html) — 比较字符串忽略案例
            *   [m2sci_strfind](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_strfind.html) — 查找一个字符串在另一个字符串
            *   [m2sci_strrep](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_strrep.html) — 字符串搜索和替换
            *   [m2sci_struct](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_struct.html) — 创建结构数组
            *   [m2sci_sum](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_sum.html) — 数组元素的总和
            *   [m2sci_surf](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_surf.html) — 三维曲面图
            *   [m2sci_svd](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_svd.html) — 奇异值分解
            *   [m2sci_switch](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_switch.html) — 在基于表达式的几个案件之间切换

                *   [T](http://help.scilab.org/docs/5.4.0/ja_JP/section_9deb26d4cb2aaee409b0fe3cfc9251f2.html)

                    *   [m2sci_tan](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_tan.html) — 切线
            *   [m2sci_tanh](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_tanh.html) — 双曲正切值
            *   [m2sci_tic](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_tic.html) — 启动秒表计时器
            *   [m2sci_title](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_title.html) — 在图形窗口中显示的标题
            *   [m2sci_toc](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_toc.html) — 读取秒表计时器
            *   [m2sci_toeplitz](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_toeplitz.html) — Toeplitz 矩阵
            *   [m2sci_tril](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_tril.html) — 矩阵的下三角部分
            *   [m2sci_triu](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_triu.html) — 三角上部的矩阵
            *   [m2sci_true](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_true.html) — 真正的数组
            *   [m2sci_type](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_type.html) — 列表文件

                *   [U](http://help.scilab.org/docs/5.4.0/ja_JP/section_379e7a7542e4250620997052184048d6.html)

                    *   [m2sci_uigetdir](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_uigetdir.html) — 选择目录的标准对话框
            *   [m2sci_uint16](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_uint16.html) — 将转换为 16 位无符号整数
            *   [m2sci_uint32](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_uint32.html) — 将转换为 32 位无符号整数
            *   [m2sci_uint8](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_uint8.html) — 将转换为 8 位无符号整数
            *   [m2sci_unix](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_unix.html) — 执行 UNIX 命令并返回结果
            *   [m2sci_upper](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_upper.html) — 将字符串转换为大写

                *   [V](http://help.scilab.org/docs/5.4.0/ja_JP/section_68f30ce57acf17ae6e5a4be6be9805b3.html)

                    *   [m2sci_varargin](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_varargin.html) — 通过可变的参数个数
            *   [m2sci_varargout](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_varargout.html) — 返回可变的参数个数
            *   [m2sci_vertcat](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_vertcat.html) — 垂直串联

                *   [Variables](http://help.scilab.org/docs/5.4.0/ja_JP/section_f12a31831e618da86b20dcf4dd6297f4.html)

                    *   [m2sci_ans](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_ans.html) — 最新的答案
            *   [m2sci_end](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_end.html) — 最后一个索引
            *   [m2sci_eps](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_eps.html) — 浮点的相对精度
            *   [m2sci_i](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_i.html) — 虚数单位
            *   [m2sci_j](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_j.html) — 虚数单位
            *   [m2sci_pi](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_pi.html) — 圆的周长与其直径的比率

                *   [W](http://help.scilab.org/docs/5.4.0/ja_JP/section_86c215d1565ee85bdd4c4f23186acb07.html)

                    *   [m2sci_waitforbuttonpress](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_waitforbuttonpress.html) — 等待键或鼠标按钮按下
            *   [m2sci_warning](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_warning.html) — 显示警告消息
            *   [m2sci_while](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_while.html) — 重复语句不定次数
            *   [m2sci_who](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_who.html) — 在工作区中的变量列表
            *   [m2sci_whos](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_whos.html) — 在工作区中的变量列表
            *   [m2sci_winqueryreg](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_winqueryreg.html) — 从 Microsoft Windows 注册表获取项目

                *   [X](http://help.scilab.org/docs/5.4.0/ja_JP/section_d143a8a22036a7f95016dcc44233cbbc.html)

                    *   [m2sci_xlabel](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_xlabel.html) — 显示一个字符串，沿 x 轴

                *   [Y](http://help.scilab.org/docs/5.4.0/ja_JP/section_ae6b511f2caf1c609dc6e35dd3f003bf.html)

                    *   [m2sci_ylabel](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_ylabel.html) — 显示一个字符串，沿 y 轴

                *   [Z](http://help.scilab.org/docs/5.4.0/ja_JP/section_fbb71d043ed78661fbd18724eb7f5f46.html)

                    *   [m2sci_zeros](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_zeros.html) — 创建全为零的数组
            *   [m2sci_zlabel](http://help.scilab.org/docs/5.4.0/ja_JP/m2sci_zlabel.html) — 显示一个字符串，沿 z 轴

        *   [About_M2SCI_tools](http://help.scilab.org/docs/5.4.0/ja_JP/About_M2SCI_tools.html) — 一般来说有关 Matlab 文件转换为 Scilab 的工具
    *   [Contents](http://help.scilab.org/docs/5.4.0/ja_JP/Contents.html) — 创建包含内容推断数据树
    *   [Cste](http://help.scilab.org/docs/5.4.0/ja_JP/Cste.html) — 创建一个目录树，表示一个常数
    *   [Equal](http://help.scilab.org/docs/5.4.0/ja_JP/Equal.html) — 创建表示指令树
    *   [Funcall](http://help.scilab.org/docs/5.4.0/ja_JP/Funcall.html) — 创建表示函数调用树
    *   [Infer](http://help.scilab.org/docs/5.4.0/ja_JP/Infer.html) — 创建包含推理数据树
    *   [MatlabScilab_character_strings](http://help.scilab.org/docs/5.4.0/ja_JP/MatlabScilab_character_strings.html) — 一般来说有关......
    *   [Operation](http://help.scilab.org/docs/5.4.0/ja_JP/Operation.html) — 创建表示操作的目录树
    *   [Type](http://help.scilab.org/docs/5.4.0/ja_JP/Type.html) — 创建包含的类型推断数据树
    *   [Variable](http://help.scilab.org/docs/5.4.0/ja_JP/Variable.html) — 创建一棵树代表一个变量
    *   [get_contents_infer](http://help.scilab.org/docs/5.4.0/ja_JP/get_contents_infer.html) — 搜索"M2SCi tlist"内容中的信息
    *   [m2scideclare](http://help.scilab.org/docs/5.4.0/ja_JP/m2scideclare.html) — 给予提示，以帮助 M2SCI。
    *   [matfile2sci](http://help.scilab.org/docs/5.4.0/ja_JP/matfile2sci.html) — Matlab 5 垫文件转换为 Scilab 的二进制文件
    *   [mfile2sci](http://help.scilab.org/docs/5.4.0/ja_JP/mfile2sci.html) — MATLAB M 文件到 Scilab 转换函数
    *   [sci_files](http://help.scilab.org/docs/5.4.0/ja_JP/sci_files.html) — 如何编写转换函数
    *   [translatepaths](http://help.scilab.org/docs/5.4.0/ja_JP/translatepaths.html) — 将一组 Matlab M 文件目录转换为 Scilab

*   [Compatibility Functions](http://help.scilab.org/docs/5.4.0/ja_JP/section_485479631e03a70c2bc5e1d3b1ef95c1.html)

    *   [mtlb_mode](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_mode.html) — 像操作开关 Matlab
    *   [asciimat](http://help.scilab.org/docs/5.4.0/ja_JP/asciimat.html) — 字符串矩阵 ascii 转换
    *   [firstnonsingleton](http://help.scilab.org/docs/5.4.0/ja_JP/firstnonsingleton.html) — 查找第一个维度，而不是 1
    *   [makecell](http://help.scilab.org/docs/5.4.0/ja_JP/makecell.html) — 创建一个单元格的数组。
    *   [mstr2sci](http://help.scilab.org/docs/5.4.0/ja_JP/mstr2sci.html) — 字符矩阵转换为字符字符串矩阵
    *   [mtlb_0](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_0.html) — 非共轭 MATLAB 换位仿真功能
    *   [mtlb_a](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_a.html) — MATLAB 加法仿真功能
    *   [mtlb_all](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_all.html) — MATLAB 所有仿真功能
    *   [mtlb_any](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_any.html) — MATLAB 仿真的任何函数
    *   [mtlb_axis](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_axis.html) — MATLAB 轴仿真功能
    *   [mtlb_beta](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_beta.html) — MATLAB beta 仿真函数
    *   [mtlb_box](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_box.html) — MATLAB 框仿真功能
    *   [mtlb_close](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_close.html) — MATLAB 关闭仿真功能
    *   [mtlb_colordef](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_colordef.html) — MATLAB colordef 仿真功能
    *   [mtlb_conv](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_conv.html) — MATLAB conv 仿真功能。 此函数已过时。
    *   [mtlb_cumprod](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_cumprod.html) — MATLAB cumprod 仿真功能
    *   [mtlb_cumsum](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_cumsum.html) — MATLAB cumsum 仿真功能
    *   [mtlb_dec2hex](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_dec2hex.html) — MATLAB 仿真 dec2hex 函数
    *   [mtlb_delete](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_delete.html) — MATLAB 删除仿真功能
    *   [mtlb_diag](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_diag.html) — MATLAB diag 仿真功能
    *   [mtlb_diff](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_diff.html) — MATLAB diff 仿真功能
    *   [mtlb_dir](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_dir.html) — MATLAB 仿真 dir 函数
    *   [mtlb_double](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_double.html) — MATLAB 双仿真功能
    *   [mtlb_e](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_e.html) — MATLAB 提取仿真功能
    *   [mtlb_echo](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_echo.html) — MATLAB 回音仿真功能
    *   [mtlb_eval](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_eval.html) — MATLAB 仿真 eval 函数
    *   [mtlb_exist](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_exist.html) — MATLAB 存在仿真功能
    *   [mtlb_eye](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_eye.html) — MATLAB 眼仿真功能
    *   [mtlb_false](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_false.html) — MATLAB 虚假仿真功能
    *   [mtlb_fft](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_fft.html) — MATLAB fft 仿真功能
    *   [mtlb_fftshift](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_fftshift.html) — MATLAB fftshift 仿真功能
    *   [mtlb_find](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_find.html) — MATLAB 找到仿真功能
    *   [mtlb_findstr](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_findstr.html) — MATLAB findstr 仿真功能
    *   [mtlb_fliplr](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_fliplr.html) — MATLAB fliplr 仿真功能
    *   [mtlb_fopen](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_fopen.html) — MATLAB fopen 仿真功能
    *   [mtlb_format](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_format.html) — MATLAB 格式仿真功能
    *   [mtlb_fprintf](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_fprintf.html) — MATLAB 标准仿真功能
    *   [mtlb_fread](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_fread.html) — MATLAB 仿真 fread 函数
    *   [mtlb_fscanf](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_fscanf.html) — MATLAB 仿真 fscanf 函数
    *   [mtlb_full](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_full.html) — MATLAB 全仿真功能
    *   [mtlb_fwrite](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_fwrite.html) — MATLAB 仿真 fwrite 函数
    *   [mtlb_grid](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_grid.html) — MATLAB 网格仿真功能
    *   [mtlb_hold](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_hold.html) — MATLAB 举行仿真功能
    *   [mtlb_i](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_i.html) — MATLAB 仿真插入函数
    *   [mtlb_ifft](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_ifft.html) — MATLAB 傅立叶仿真功能
    *   [mtlb_imp](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_imp.html) — MATLAB 结肠仿真功能
    *   [mtlb_int16](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_int16.html) — MATLAB int16 仿真功能
    *   [mtlb_int32](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_int32.html) — MATLAB int32 仿真功能
    *   [mtlb_int8](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_int8.html) — MATLAB int8 仿真功能
    *   [mtlb_is](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_is.html) — MATLAB 字符串插入仿真功能
    *   [mtlb_isa](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_isa.html) — MATLAB isa 仿真功能
    *   [mtlb_isfield](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_isfield.html) — MATLAB isfield 仿真功能
    *   [mtlb_isletter](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_isletter.html) — MATLAB isletter 仿真功能
    *   [mtlb_isspace](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_isspace.html) — MATLAB isspace 仿真功能
    *   [mtlb_l](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_l.html) — MATLAB 左司仿真功能
    *   [mtlb_legendre](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_legendre.html) — MATLAB 仿真勒让德函数
    *   [mtlb_linspace](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_linspace.html) — MATLAB linspace 仿真功能
    *   [mtlb_logic](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_logic.html) — MATLAB 仿真逻辑运算符函数
    *   [mtlb_logical](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_logical.html) — MATLAB 仿真逻辑函数
    *   [mtlb_lower](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_lower.html) — MATLAB 低仿真功能
    *   [mtlb_max](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_max.html) — MATLAB 最大仿真功能
    *   [mtlb_min](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_min.html) — MATLAB 仿真 min 函数
    *   [mtlb_more](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_more.html) — MATLAB 仿真功能更多
    *   [mtlb_num2str](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_num2str.html) — MATLAB num2str 仿真功能
    *   [mtlb_ones](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_ones.html) — MATLAB 的仿真功能
    *   [mtlb_plot](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_plot.html) — MATLAB 绘图仿真功能
    *   [mtlb_prod](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_prod.html) — MATLAB 督促仿真功能
    *   [mtlb_rand](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_rand.html) — MATLAB 仿真 rand 函数
    *   [mtlb_randn](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_randn.html) — MATLAB randn 仿真功能
    *   [mtlb_rcond](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_rcond.html) — MATLAB rcond 仿真功能
    *   [mtlb_realmax](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_realmax.html) — MATLAB realmax 仿真功能
    *   [mtlb_realmin](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_realmin.html) — MATLAB realmin 仿真功能
    *   [mtlb_repmat](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_repmat.html) — MATLAB repmat 仿真功能
    *   [mtlb_s](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_s.html) — MATLAB 减影仿真功能
    *   [mtlb_setstr](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_setstr.html) — MATLAB setstr 仿真功能
    *   [mtlb_size](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_size.html) — MATLAB 大小仿真功能
    *   [mtlb_sort](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_sort.html) — MATLAB 仿真排序函数
    *   [mtlb_strcmp](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_strcmp.html) — MATLAB 仿真 strcmp 函数
    *   [mtlb_strcmpi](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_strcmpi.html) — MATLAB strcmpi 仿真功能
    *   [mtlb_strfind](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_strfind.html) — MATLAB strfind 仿真功能
    *   [mtlb_strrep](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_strrep.html) — MATLAB strrep 仿真功能
    *   [mtlb_sum](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_sum.html) — MATLAB 仿真 sum 函数
    *   [mtlb_t](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_t.html) — MATLAB 换位仿真功能
    *   [mtlb_toeplitz](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_toeplitz.html) — MATLAB toeplitz 仿真功能
    *   [mtlb_tril](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_tril.html) — MATLAB 创富仿真功能
    *   [mtlb_triu](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_triu.html) — MATLAB triu 仿真功能
    *   [mtlb_true](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_true.html) — MATLAB 真实仿真功能
    *   [mtlb_uint16](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_uint16.html) — MATLAB uint16 仿真功能
    *   [mtlb_uint32](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_uint32.html) — MATLAB uint32 仿真功能
    *   [mtlb_uint8](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_uint8.html) — MATLAB uint8 仿真功能
    *   [mtlb_upper](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_upper.html) — MATLAB 上部仿真功能
    *   [mtlb_var](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_var.html) — MATLAB 仿真 var 函数
    *   [mtlb_zeros](http://help.scilab.org/docs/5.4.0/ja_JP/mtlb_zeros.html) — MATLAB 零仿真功能

*   高级函数[Advanced functions](http://help.scilab.org/docs/5.4.0/ja_JP/section_997d85f1e858acd27522a1ca8c0dbff6.html)

    *   [Built-in &amp; external](http://help.scilab.org/docs/5.4.0/ja_JP/section_043938404b903a6ad7c2ebd9ea31d26b.html)

            *   [clearfun](http://help.scilab.org/docs/5.4.0/ja_JP/clearfun.html) — 删除原始 （内置函数）
        *   [external](http://help.scilab.org/docs/5.4.0/ja_JP/external.html) — Scilab 对象、 外部函数或例程
        *   [funptr](http://help.scilab.org/docs/5.4.0/ja_JP/funptr.html) — Primitives 的编码 （高级的用户）
        *   [intppty](http://help.scilab.org/docs/5.4.0/ja_JP/intppty.html) — 指定指定属性的接口参数
        *   [newfun](http://help.scilab.org/docs/5.4.0/ja_JP/newfun.html) — 将名称添加到函数表
        *   [readgateway](http://help.scilab.org/docs/5.4.0/ja_JP/readgateway.html) — 列表的模块 primitives
        *   [what](http://help.scilab.org/docs/5.4.0/ja_JP/what.html) — Scilab primitives 的列表

        *   [Libraries](http://help.scilab.org/docs/5.4.0/ja_JP/section_a1018202eccd63401cb5e7fc4dc2e446.html)

            *   [genlib](http://help.scilab.org/docs/5.4.0/ja_JP/genlib.html) — 若要生成指定的目录中的库函数
        *   [get_function_path](http://help.scilab.org/docs/5.4.0/ja_JP/get_function_path.html) — 获取库函数中的源文件的路径
        *   [lib](http://help.scilab.org/docs/5.4.0/ja_JP/lib.html) — 库定义
        *   [librarieslist](http://help.scilab.org/docs/5.4.0/ja_JP/librarieslist.html) — 获取 scilab 图书馆
        *   [library](http://help.scilab.org/docs/5.4.0/ja_JP/library.html) — 库数据类型说明
        *   [libraryinfo](http://help.scilab.org/docs/5.4.0/ja_JP/libraryinfo.html) — 获取对宏和 scilab 的库路径
        *   [whereis](http://help.scilab.org/docs/5.4.0/ja_JP/whereis.html) — 属于该函数库的名称

        *   [profiling](http://help.scilab.org/docs/5.4.0/ja_JP/section_b5cc33710e798bc44f2d4efcd28dabf1.html)

            *   [add_profiling](http://help.scilab.org/docs/5.4.0/ja_JP/add_profiling.html) — 将配置文件命令添加到函数。
        *   [plotprofile](http://help.scilab.org/docs/5.4.0/ja_JP/plotprofile.html) — 若要查看，部署 Scilab 函数的配置文件
        *   [profile](http://help.scilab.org/docs/5.4.0/ja_JP/profile.html) — Scilab 函数的配置文件作为扩大运行
        *   [remove_profiling](http://help.scilab.org/docs/5.4.0/ja_JP/remove_profiling.html) — 若要删除的配置文件顺序功能。
        *   [reset_profiling](http://help.scilab.org/docs/5.4.0/ja_JP/reset_profiling.html) — 重置性能分析计数器功能
        *   [showprofile](http://help.scilab.org/docs/5.4.0/ja_JP/showprofile.html) — 若要查看，扩大运行 Scilab 函数的配置文件作为

        *   [argn](http://help.scilab.org/docs/5.4.0/ja_JP/argn.html) — 返回的函数调用的输入 / 输出参数的数目
    *   [bytecode](http://help.scilab.org/docs/5.4.0/ja_JP/bytecode.html) — 或到 Scilab 数组指定 Scilab 函数的相反过程返回"字节代码"，......
    *   [bytecodewalk](http://help.scilab.org/docs/5.4.0/ja_JP/bytecodewalk.html) — 若要翻译，搜索功能字节代码。
    *   [comp](http://help.scilab.org/docs/5.4.0/ja_JP/comp.html) — scilab 函数编译
    *   [deff](http://help.scilab.org/docs/5.4.0/ja_JP/deff.html) — 在线定义的函数
    *   [edit](http://help.scilab.org/docs/5.4.0/ja_JP/edit.html) — 编辑功能
    *   [exec](http://help.scilab.org/docs/5.4.0/ja_JP/exec.html) —  按顺序执行文件中所包含的Scilab指令
    *   [execstr](http://help.scilab.org/docs/5.4.0/ja_JP/execstr.html) — 执行字符串中的Scilab 代码
    *   [fun2string](http://help.scilab.org/docs/5.4.0/ja_JP/fun2string.html) — 生成 ASCII Scilab 函数的定义
    *   [funcprot](http://help.scilab.org/docs/5.4.0/ja_JP/funcprot.html) — Scilab 函数保护模式切换
    *   [function](http://help.scilab.org/docs/5.4.0/ja_JP/function.html) — 关闭函数定义
    *   [functions](http://help.scilab.org/docs/5.4.0/ja_JP/functions.html) — Scilab 程序和 Scilab 对象
    *   [getd](http://help.scilab.org/docs/5.4.0/ja_JP/getd.html) — 要在目录中定义的所有功能
    *   [head_comments](http://help.scilab.org/docs/5.4.0/ja_JP/head_comments.html) — 显示 Scilab 函数头注释
    *   [listfunctions](http://help.scilab.org/docs/5.4.0/ja_JP/listfunctions.html) — 工作区属性的所有功能
    *   [macr2lst](http://help.scilab.org/docs/5.4.0/ja_JP/macr2lst.html) — 转换函数的列表
    *   [macr2tree](http://help.scilab.org/docs/5.4.0/ja_JP/macr2tree.html) — 树转换函数
    *   [macro](http://help.scilab.org/docs/5.4.0/ja_JP/macro.html) — Scilab 程序和 Scilab 对象
    *   [macrovar](http://help.scilab.org/docs/5.4.0/ja_JP/macrovar.html) — 函数变量
    *   [mode](http://help.scilab.org/docs/5.4.0/ja_JP/mode.html) — 选择运行文件模式
    *   [overloading](http://help.scilab.org/docs/5.4.0/ja_JP/overloading.html) — 显示、 函数和运算符重载的能力
    *   [recompilefunction](http://help.scilab.org/docs/5.4.0/ja_JP/recompilefunction.html) — 若要更改的类型，重新编译 Scilab 函数
    *   [sciargs](http://help.scilab.org/docs/5.4.0/ja_JP/sciargs.html) — Scilab 命令行参数
    *   [tree2code](http://help.scilab.org/docs/5.4.0/ja_JP/tree2code.html) — 生成 ASCII Scilab 函数的定义
    *   [varargin](http://help.scilab.org/docs/5.4.0/ja_JP/varargin.html) — 到输入的参数列表中的参数数目可变
    *   [varargout](http://help.scilab.org/docs/5.4.0/ja_JP/varargout.html) — 输出变量列表中的参数的变量数
    *   [code2str](http://help.scilab.org/docs/5.4.0/ja_JP/code2str.html) — 返回的字符与 Scilab 整数代码关联的字符串。 此函数已过时。
    *   [str2code](http://help.scilab.org/docs/5.4.0/ja_JP/str2code.html) — 返回 scilab 整数代码关联的字符的字符串。 此函数已过时。

*   开发工具[Development tools](http://help.scilab.org/docs/5.4.0/ja_JP/section_8526fd323d6776f8151293d3007d1dea.html)

    *   [Assert](http://help.scilab.org/docs/5.4.0/ja_JP/section_c48fcaeb75216628502d2e4816096da2.html)

            *   [assert_overview](http://help.scilab.org/docs/5.4.0/ja_JP/assert_overview.html) — Assert 模块的概览。
        *   [assert_checkalmostequal](http://help.scilab.org/docs/5.4.0/ja_JP/assert_checkalmostequal.html) — 检查，计算和预期是按数字顺序密切。
        *   [assert_checkequal](http://help.scilab.org/docs/5.4.0/ja_JP/assert_checkequal.html) — 检查，计算和预期是平等的。
        *   [assert_checkerror](http://help.scilab.org/docs/5.4.0/ja_JP/assert_checkerror.html) — 检查指令产生预期的错误。
        *   [assert_checkfalse](http://help.scilab.org/docs/5.4.0/ja_JP/assert_checkfalse.html) — 请检查该条件为 false。
        *   [assert_checkfilesequal](http://help.scilab.org/docs/5.4.0/ja_JP/assert_checkfilesequal.html) — 检查两个文件是平等。
        *   [assert_checktrue](http://help.scilab.org/docs/5.4.0/ja_JP/assert_checktrue.html) — 检查条件为 true。
        *   [assert_comparecomplex](http://help.scilab.org/docs/5.4.0/ja_JP/assert_comparecomplex.html) — 比较复杂的数字与宽容。
        *   [assert_computedigits](http://help.scilab.org/docs/5.4.0/ja_JP/assert_computedigits.html) — 返回计算结果中的数字位数。
        *   [assert_cond2reltol](http://help.scilab.org/docs/5.4.0/ja_JP/assert_cond2reltol.html) — 表明相对误差，计算出的条件数。
        *   [assert_cond2reqdigits](http://help.scilab.org/docs/5.4.0/ja_JP/assert_cond2reqdigits.html) — 表明所需的位数，给予的条件数。
        *   [assert_generror](http://help.scilab.org/docs/5.4.0/ja_JP/assert_generror.html) — 将生成一个错误。

        *   [user](http://help.scilab.org/docs/5.4.0/ja_JP/user.html) — 为 Fortran 或 C 例程创建界面
    *   [bench_run](http://help.scilab.org/docs/5.4.0/ja_JP/bench_run.html) — 启动基准测试
    *   [example_run](http://help.scilab.org/docs/5.4.0/ja_JP/example_run.html) — 启动帮助页中找到的示例。
    *   [test_run](http://help.scilab.org/docs/5.4.0/ja_JP/test_run.html) — 启动测试

*   演示工具[Demo Tools](http://help.scilab.org/docs/5.4.0/ja_JP/section_4f8b685c702f81cc352fea32c1095b11.html)

    *   [add_demo](http://help.scilab.org/docs/5.4.0/ja_JP/add_demo.html) — 将条目添加到 デモリスト
    *   [demo_begin](http://help.scilab.org/docs/5.4.0/ja_JP/demo_begin.html) — 开始演示
    *   [demo_choose](http://help.scilab.org/docs/5.4.0/ja_JP/demo_choose.html) — 创建一个对话框供选择的选项
    *   [demo_compiler](http://help.scilab.org/docs/5.4.0/ja_JP/demo_compiler.html) — 测试 compileur 的存在
    *   [demo_end](http://help.scilab.org/docs/5.4.0/ja_JP/demo_end.html) — 完成示范
    *   [demo_file_choice](http://help.scilab.org/docs/5.4.0/ja_JP/demo_file_choice.html) — 选择并执行列表中的项
    *   [demo_function_choice](http://help.scilab.org/docs/5.4.0/ja_JP/demo_function_choice.html) — 选择并执行列表中的项
    *   [demo_mdialog](http://help.scilab.org/docs/5.4.0/ja_JP/demo_mdialog.html) — 创建一个对话框
    *   [demo_message](http://help.scilab.org/docs/5.4.0/ja_JP/demo_message.html) — 显示一条消息
    *   [demo_run](http://help.scilab.org/docs/5.4.0/ja_JP/demo_run.html) — 脚本文件执行

*   动态/增量链接[Dynamic/incremental Link](http://help.scilab.org/docs/5.4.0/ja_JP/section_90d493bb565dbb3267b3f1369cbed780.html)

    *   [G_make](http://help.scilab.org/docs/5.4.0/ja_JP/G_make.html) — 使或 nmake 调用
    *   [addinter](http://help.scilab.org/docs/5.4.0/ja_JP/addinter.html) — 新的函数接口在运行时动态链接。
    *   [c_link](http://help.scilab.org/docs/5.4.0/ja_JP/c_link.html) — 检查是否符号加载与动态链接
    *   [call](http://help.scilab.org/docs/5.4.0/ja_JP/call.html) — Fortran 或 C 用户例程调用
    *   [chooselcccompiler](http://help.scilab.org/docs/5.4.0/ja_JP/chooselcccompiler.html) — 移动作为原子中的工具箱
    *   [configure_msifort](http://help.scilab.org/docs/5.4.0/ja_JP/configure_msifort.html) — 为英特尔 Fortran 编译器 (Windows) 设置环境变量。
    *   [configure_msvc](http://help.scilab.org/docs/5.4.0/ja_JP/configure_msvc.html) — 为 Microsoft C 编译器设置的环境变量。
    *   [dllinfo](http://help.scilab.org/docs/5.4.0/ja_JP/dllinfo.html) — 提供了有关格式和符号的可执行文件和 DLL 文件 (Windows) 中提供的信息。
    *   [findmsifortcompiler](http://help.scilab.org/docs/5.4.0/ja_JP/findmsifortcompiler.html) — 检测到英特尔 fortran 编译器
    *   [findmsvccompiler](http://help.scilab.org/docs/5.4.0/ja_JP/findmsvccompiler.html) — 检测到 Microsoft C 编译器
    *   [fort](http://help.scilab.org/docs/5.4.0/ja_JP/fort.html) — Fortran 或 C 用户例程调用
    *   [getdynlibext](http://help.scilab.org/docs/5.4.0/ja_JP/getdynlibext.html) — 获取关于您的操作系统的动态库的扩展名。
    *   [haveacompiler](http://help.scilab.org/docs/5.4.0/ja_JP/haveacompiler.html) — 检测如果你有一个 C 编译器。
    *   [ilib_build](http://help.scilab.org/docs/5.4.0/ja_JP/ilib_build.html) — 用于共享的库管理实用程序
    *   [ilib_compile](http://help.scilab.org/docs/5.4.0/ja_JP/ilib_compile.html) — ilib_build 实用程序： 执行生成文件中产生的 ilib_gen_Make
    *   [ilib_for_link](http://help.scilab.org/docs/5.4.0/ja_JP/ilib_for_link.html) — 实用程序，用于与链接的共享的库管理
    *   [ilib_gen_Make](http://help.scilab.org/docs/5.4.0/ja_JP/ilib_gen_Make.html) — ilib_build 实用程序： 用于构建共享的库生成生成文件
    *   [ilib_gen_cleaner](http://help.scilab.org/docs/5.4.0/ja_JP/ilib_gen_cleaner.html) — ilib_build 实用程序： 生成一个更清洁的文件
    *   [ilib_gen_gateway](http://help.scilab.org/docs/5.4.0/ja_JP/ilib_gen_gateway.html) — 用于 ilib_build，实用程序会生成一个网关文件。
    *   [ilib_gen_loader](http://help.scilab.org/docs/5.4.0/ja_JP/ilib_gen_loader.html) — ilib_build 实用程序： 生成一个加载程序文件
    *   [ilib_include_flag](http://help.scilab.org/docs/5.4.0/ja_JP/ilib_include_flag.html) — 返回格式化包含要传递到系统编译器的相关的字符串
    *   [ilib_mex_build](http://help.scilab.org/docs/5.4.0/ja_JP/ilib_mex_build.html) — 墨西哥图书馆管理的实用程序
    *   [ilib_verbose](http://help.scilab.org/docs/5.4.0/ja_JP/ilib_verbose.html) — 设置显示动态链接函数使用的等级。
    *   [link](http://help.scilab.org/docs/5.4.0/ja_JP/link.html) — 动态链接器
    *   [supported_compilers](http://help.scilab.org/docs/5.4.0/ja_JP/supported_compilers.html) — 支持和兼容的编译器，由 Scilab
    *   [ulink](http://help.scilab.org/docs/5.4.0/ja_JP/ulink.html) — 取消动态链接的共享的对象的链接

*   [Atoms](http://help.scilab.org/docs/5.4.0/ja_JP/section_c0fe6327d3fd3707b5289eac5c42a687.html)

    *   [_atomsGettingStarted](http://help.scilab.org/docs/5.4.0/ja_JP/_atomsGettingStarted.html) —
    *   [atoms](http://help.scilab.org/docs/5.4.0/ja_JP/atoms.html) —
    *   [atomsAutoload](http://help.scilab.org/docs/5.4.0/ja_JP/atomsAutoload.html) — 加载标记为"自动"加载的模块
    *   [atomsAutoloadAdd](http://help.scilab.org/docs/5.4.0/ja_JP/atomsAutoloadAdd.html) — 将一个或几个模块添加到自动加载
    *   [atomsAutoloadDel](http://help.scilab.org/docs/5.4.0/ja_JP/atomsAutoloadDel.html) — 从自动加载系统中删除的一个或几个模块
    *   [atomsAutoloadList](http://help.scilab.org/docs/5.4.0/ja_JP/atomsAutoloadList.html) — 获取注册到自动加载的模块的列表
    *   [atomsCategoryList](http://help.scilab.org/docs/5.4.0/ja_JP/atomsCategoryList.html) — 可用类别的列表
    *   [atomsCheckModule](http://help.scilab.org/docs/5.4.0/ja_JP/atomsCheckModule.html) — 检查给定的原子模块列表
    *   [atomsDepTreeShow](http://help.scilab.org/docs/5.4.0/ja_JP/atomsDepTreeShow.html) — 显示模块的依赖关系树
    *   [atomsGetConfig](http://help.scilab.org/docs/5.4.0/ja_JP/atomsGetConfig.html) — 获得原子系统参数
    *   [atomsGetInstalled](http://help.scilab.org/docs/5.4.0/ja_JP/atomsGetInstalled.html) — 获取已安装外部模块的列表
    *   [atomsGetInstalledPath](http://help.scilab.org/docs/5.4.0/ja_JP/atomsGetInstalledPath.html) — 获取已安装外部模块的安装路径
    *   [atomsGetLoaded](http://help.scilab.org/docs/5.4.0/ja_JP/atomsGetLoaded.html) — 获取已加载的外部模块的列表
    *   [atomsGetLoadedPath](http://help.scilab.org/docs/5.4.0/ja_JP/atomsGetLoadedPath.html) — 返回已加载外部模块的安装目录的路径。
    *   [atomsInstall](http://help.scilab.org/docs/5.4.0/ja_JP/atomsInstall.html) — 安装一个或多个外部模块
    *   [atomsIsInstalled](http://help.scilab.org/docs/5.4.0/ja_JP/atomsIsInstalled.html) — 确定是否已安装该模块。 如果模块是安装，否则为 false，则返回 true。
    *   [atomsIsLoaded](http://help.scilab.org/docs/5.4.0/ja_JP/atomsIsLoaded.html) — 决定是否进行或不加载的模块
    *   [atomsList](http://help.scilab.org/docs/5.4.0/ja_JP/atomsList.html) — 列表中可用的外部模块
    *   [atomsLoad](http://help.scilab.org/docs/5.4.0/ja_JP/atomsLoad.html) — 加载外部的一个或几个模块
    *   [atomsQuit](http://help.scilab.org/docs/5.4.0/ja_JP/atomsQuit.html) — 以前加载的原子 （Call.quit 文件） 卸载外部模块
    *   [atomsRemove](http://help.scilab.org/docs/5.4.0/ja_JP/atomsRemove.html) — 删除一个或几个模块
    *   [atomsRepositoryAdd](http://help.scilab.org/docs/5.4.0/ja_JP/atomsRepositoryAdd.html) — 向托管资料库列表中添加一个或多个 Url
    *   [atomsRepositoryDel](http://help.scilab.org/docs/5.4.0/ja_JP/atomsRepositoryDel.html) — 从托管资料库列表中删除一个或多个 Url
    *   [atomsRepositoryList](http://help.scilab.org/docs/5.4.0/ja_JP/atomsRepositoryList.html) — 获取托管资料库列表中
    *   [atomsRestoreConfig](http://help.scilab.org/docs/5.4.0/ja_JP/atomsRestoreConfig.html) — 从备份文件还原配置
    *   [atomsSaveConfig](http://help.scilab.org/docs/5.4.0/ja_JP/atomsSaveConfig.html) — 使配置文件的备份
    *   [atomsSearch](http://help.scilab.org/docs/5.4.0/ja_JP/atomsSearch.html) — 搜索外部模块。
    *   [atomsSetConfig](http://help.scilab.org/docs/5.4.0/ja_JP/atomsSetConfig.html) — 管理原子系统参数
    *   [atomsShow](http://help.scilab.org/docs/5.4.0/ja_JP/atomsShow.html) — 显示模块的特点
    *   [atomsSystemInit](http://help.scilab.org/docs/5.4.0/ja_JP/atomsSystemInit.html) — 设置为原子系统应有的写访问权限
    *   [atomsSystemUpdate](http://help.scilab.org/docs/5.4.0/ja_JP/atomsSystemUpdate.html) — 更新可用的模块的列表
    *   [atomsTest](http://help.scilab.org/docs/5.4.0/ja_JP/atomsTest.html) — 执行给定的测试安装模块
    *   [atomsUpdate](http://help.scilab.org/docs/5.4.0/ja_JP/atomsUpdate.html) — 更新一个或多个外部模块
    *   [atomsVersion](http://help.scilab.org/docs/5.4.0/ja_JP/atomsVersion.html) — 显示 Scilab 的原子版本

*   Tcl/Tk 接口[Tcl/Tk Interface](http://help.scilab.org/docs/5.4.0/ja_JP/section_b742f9e4194f63cadf7d0059440c5e02.html)

    *   [ScilabEval](http://help.scilab.org/docs/5.4.0/ja_JP/ScilabEval.html) — Tcl 指令： scilab 译员与评估字符串
    *   [TCL_CreateSlave](http://help.scilab.org/docs/5.4.0/ja_JP/TCL_CreateSlave.html) — 创建一个 TCL 奴隶解释器
    *   [TCL_DeleteInterp](http://help.scilab.org/docs/5.4.0/ja_JP/TCL_DeleteInterp.html) — 删除 TCL 解释器
    *   [TCL_EvalFile](http://help.scilab.org/docs/5.4.0/ja_JP/TCL_EvalFile.html) — 读取并评估 Tcl/Tk 的文件
    *   [TCL_EvalStr](http://help.scilab.org/docs/5.4.0/ja_JP/TCL_EvalStr.html) — 评估字符串中等 TCL/TK 译员
    *   [TCL_ExistArray](http://help.scilab.org/docs/5.4.0/ja_JP/TCL_ExistArray.html) — 如果存在一个 tcl 数组，返回 %T
    *   [TCL_ExistInterp](http://help.scilab.org/docs/5.4.0/ja_JP/TCL_ExistInterp.html) — 如果 tcl 奴隶口笔译存在，则返回 %T
    *   [TCL_ExistVar](http://help.scilab.org/docs/5.4.0/ja_JP/TCL_ExistVar.html) — 如果存在 tcl 变量，返回 %T
    *   [TCL_GetVar](http://help.scilab.org/docs/5.4.0/ja_JP/TCL_GetVar.html) — 获取一个 Tcl/Tk 的变量值
    *   [TCL_GetVersion](http://help.scilab.org/docs/5.4.0/ja_JP/TCL_GetVersion.html) — 获取在运行时的 TCL/TK 库的版本。
    *   [TCL_SetVar](http://help.scilab.org/docs/5.4.0/ja_JP/TCL_SetVar.html) — 设置了 Tcl/Tk 的变量值
    *   [TCL_UnsetVar](http://help.scilab.org/docs/5.4.0/ja_JP/TCL_UnsetVar.html) — 删除 tcl 变量
    *   [TCL_UpVar](http://help.scilab.org/docs/5.4.0/ja_JP/TCL_UpVar.html) — 使从 tcl 源变量到 tcl 目标变量的链接
    *   [config](http://help.scilab.org/docs/5.4.0/ja_JP/config.html) — Scilab 常规配置。 此函数已过时。
    *   [winclose](http://help.scilab.org/docs/5.4.0/ja_JP/winclose.html) — 关闭 windows 创建的 sciGUI
    *   [winlist](http://help.scilab.org/docs/5.4.0/ja_JP/winlist.html) — 返回当前窗口创建的 sciGUI 的振荡

*   scilab编辑器[scilab editor](http://help.scilab.org/docs/5.4.0/ja_JP/section_59cde36a132b0630deac8aca34aff288.html)

    *   [edit_error](http://help.scilab.org/docs/5.4.0/ja_JP/edit_error.html) — 打开 scilab 编辑器中的最后一个记录错误
    *   [editor](http://help.scilab.org/docs/5.4.0/ja_JP/editor.html) — 要调用文本编辑器，它由定义的
    *   [scinotes](http://help.scilab.org/docs/5.4.0/ja_JP/scinotes.html) — Scinotes: Scilab 嵌入的文本编辑器

*   UI数据[UI Data](http://help.scilab.org/docs/5.4.0/ja_JP/section_d5c3a9358485a79e4fd71849b836ffc0.html)

    *   [browsevar](http://help.scilab.org/docs/5.4.0/ja_JP/browsevar.html) — Scilab 变量浏览器
    *   [editvar](http://help.scilab.org/docs/5.4.0/ja_JP/editvar.html) — Scilab 变量编辑器
    *   [filebrowser](http://help.scilab.org/docs/5.4.0/ja_JP/filebrowser.html) — 打开 Scilab ファイルブラウザ

*   在线帮助管理[Online help management](http://help.scilab.org/docs/5.4.0/ja_JP/section_9a31915dc7c2d72eddaee1b92b622aa5.html)

    *   [add_help_chapter](http://help.scilab.org/docs/5.4.0/ja_JP/add_help_chapter.html) — 为帮助列表中添加一个条目
    *   [apropos](http://help.scilab.org/docs/5.4.0/ja_JP/apropos.html) — Scilab 帮助中搜索关键字
    *   [del_help_chapter](http://help.scilab.org/docs/5.4.0/ja_JP/del_help_chapter.html) — 删除帮助列表中的条目
    *   [help](http://help.scilab.org/docs/5.4.0/ja_JP/help.html) — 在线帮助命令
    *   [help_from_sci](http://help.scilab.org/docs/5.4.0/ja_JP/help_from_sci.html) — 从 a.sci 源文件的头部注释部分生成帮助文件和演示文件。
    *   [help_skeleton](http://help.scilab.org/docs/5.4.0/ja_JP/help_skeleton.html) — 生成到 Scilab 函数相关联的 xml 帮助文件的骨架
    *   [how_to_link_toolbox_help](http://help.scilab.org/docs/5.4.0/ja_JP/how_to_link_toolbox_help.html) — 如何使工具箱帮助指向 Scilab 的项目中的超链接
    *   [man](http://help.scilab.org/docs/5.4.0/ja_JP/man.html) — 行上帮助 XML 文件格式说明
    *   [manedit](http://help.scilab.org/docs/5.4.0/ja_JP/manedit.html) — 编辑手动项
    *   [percenthelps](http://help.scilab.org/docs/5.4.0/ja_JP/percenthelps.html) — 变量定义的帮助目录的路径
    *   [xmltochm](http://help.scilab.org/docs/5.4.0/ja_JP/xmltochm.html) — 将 xml Scilab 帮助文件转换为 Microsoft 压缩 HTML 格式 (Windows)
    *   [xmltohtml](http://help.scilab.org/docs/5.4.0/ja_JP/xmltohtml.html) — 将 xml Scilab 帮助文件转换为 HTML 格式
    *   [xmltojar](http://help.scilab.org/docs/5.4.0/ja_JP/xmltojar.html) — 将 xml Scilab 帮助文件转换为 javaHelp 格式
    *   [xmltopdf](http://help.scilab.org/docs/5.4.0/ja_JP/xmltopdf.html) — 将 xml Scilab 帮助文件转换为 pdf 格式
    *   [xmltops](http://help.scilab.org/docs/5.4.0/ja_JP/xmltops.html) — 将 xml Scilab 帮助文件转换为 postscript 格式

*   并行运算[Parallel](http://help.scilab.org/docs/5.4.0/ja_JP/section_76cc9ff7f25c1f0b2d5e17570c77897d.html)

    *   [parallel_concurrency](http://help.scilab.org/docs/5.4.0/ja_JP/parallel_concurrency.html) — 关于当前执行上下文的并发查询
    *   [parallel_run](http://help.scilab.org/docs/5.4.0/ja_JP/parallel_run.html) — 并行调用函数

*   模块管理[Modules manager](http://help.scilab.org/docs/5.4.0/ja_JP/section_595ae4a5f9d5e2c99f85e11a58238003.html)

    *   [tbx_build_blocks](http://help.scilab.org/docs/5.4.0/ja_JP/tbx_build_blocks.html) — 编译块 （工具箱编译过程）
    *   [tbx_build_cleaner](http://help.scilab.org/docs/5.4.0/ja_JP/tbx_build_cleaner.html) — 生成一个 cleaner.sce 脚本 （工具箱编译过程）
    *   [tbx_build_gateway](http://help.scilab.org/docs/5.4.0/ja_JP/tbx_build_gateway.html) — 建立一个网关 （工具箱编译过程）
    *   [tbx_build_gateway_clean](http://help.scilab.org/docs/5.4.0/ja_JP/tbx_build_gateway_clean.html) — 生成一个 cleaner_gateway.sce 脚本 （工具箱编译过程）
    *   [tbx_build_gateway_loader](http://help.scilab.org/docs/5.4.0/ja_JP/tbx_build_gateway_loader.html) — 生成一个 loader_gateway.sce 脚本 （工具箱编译过程）
    *   [tbx_build_help](http://help.scilab.org/docs/5.4.0/ja_JP/tbx_build_help.html) — 生成帮助文件 （工具箱编译过程）
    *   [tbx_build_help_loader](http://help.scilab.org/docs/5.4.0/ja_JP/tbx_build_help_loader.html) — 生成 addchapter.sce 脚本 （工具箱编译过程）
    *   [tbx_build_loader](http://help.scilab.org/docs/5.4.0/ja_JP/tbx_build_loader.html) — 生成 loader.sce 和卸机脚本 （工具箱编译过程）
    *   [tbx_build_macros](http://help.scilab.org/docs/5.4.0/ja_JP/tbx_build_macros.html) — 编译宏 （工具箱编译过程）
    *   [tbx_build_src](http://help.scilab.org/docs/5.4.0/ja_JP/tbx_build_src.html) — 生成来源 （工具箱编译过程）
    *   [tbx_builder_gateway](http://help.scilab.org/docs/5.4.0/ja_JP/tbx_builder_gateway.html) — 运行 builder_gateway.sce 脚本，如果它存在 （工具箱编译过程）
    *   [tbx_builder_gateway_lang](http://help.scilab.org/docs/5.4.0/ja_JP/tbx_builder_gateway_lang.html) — 运行 builder_gateway_ （语言）.sce 脚本，如果它存在 （工具箱编译过程）
    *   [tbx_builder_help](http://help.scilab.org/docs/5.4.0/ja_JP/tbx_builder_help.html) — 运行 builder_help.sce 脚本，如果它存在 （工具箱编译过程）
    *   [tbx_builder_help_lang](http://help.scilab.org/docs/5.4.0/ja_JP/tbx_builder_help_lang.html) — 运行 build_help.sce 脚本，如果它存在 （工具箱编译过程）
    *   [tbx_builder_macros](http://help.scilab.org/docs/5.4.0/ja_JP/tbx_builder_macros.html) — 运行 buildmacros.sce 脚本，如果它存在 （工具箱编译过程）
    *   [tbx_builder_src](http://help.scilab.org/docs/5.4.0/ja_JP/tbx_builder_src.html) — 运行 builder_src.sce 脚本，如果它存在 （工具箱编译过程）
    *   [tbx_builder_src_lang](http://help.scilab.org/docs/5.4.0/ja_JP/tbx_builder_src_lang.html) — 运行 builder_ （语言）.sce 脚本，如果它存在 （工具箱编译过程）

*   本地化[Localization](http://help.scilab.org/docs/5.4.0/ja_JP/section_f7bbdcf2f95141ec61d60b1c4bcb3781.html)

    *   [dgettext](http://help.scilab.org/docs/5.4.0/ja_JP/dgettext.html) — 获取文本译成当前的区域设置和特定的域
    *   [getdefaultlanguage](http://help.scilab.org/docs/5.4.0/ja_JP/getdefaultlanguage.html) — 返回由 Scilab 使用的默认语言
    *   [getlanguage](http://help.scilab.org/docs/5.4.0/ja_JP/getlanguage.html) — 返回由 Scilab 使用的当前语言。
    *   [gettext](http://help.scilab.org/docs/5.4.0/ja_JP/gettext.html) — 类似于 gettext
    *   [LANGUAGE](http://help.scilab.org/docs/5.4.0/ja_JP/LANGUAGE.html) — 变量定义的语言 （已过时）
    *   [setdefaultlanguage](http://help.scilab.org/docs/5.4.0/ja_JP/setdefaultlanguage.html) — 设置和保存的内部语言值。
    *   [setlanguage](http://help.scilab.org/docs/5.4.0/ja_JP/setlanguage.html) — 设置的内部语言值 （仅限 Windows）

*   Java虚拟机[JVM](http://help.scilab.org/docs/5.4.0/ja_JP/section_d0c301ad9c2e85f6c2ea289661323f64.html)

    *   [javaclasspath](http://help.scilab.org/docs/5.4.0/ja_JP/javaclasspath.html) — 集和获取动态 Java 类路径
    *   [javalibrarypath](http://help.scilab.org/docs/5.4.0/ja_JP/javalibrarypath.html) — 设置和获取动态 java.library.path
    *   [jre_path](http://help.scilab.org/docs/5.4.0/ja_JP/jre_path.html) — 返回由 Scilab 使用的 Java 运行时环境
    *   [system_getproperty](http://help.scilab.org/docs/5.4.0/ja_JP/system_getproperty.html) — 获取由指定的键指示的系统属性。
    *   [system_setproperty](http://help.scilab.org/docs/5.4.0/ja_JP/system_setproperty.html) — 设置系统属性，表示由指定的键和值。
    *   [with_embedded_jre](http://help.scilab.org/docs/5.4.0/ja_JP/with_embedded_jre.html) — 检查 scilab 是否使用嵌入的 JRE

*   [API Scilab](http://help.scilab.org/docs/5.4.0/ja_JP/section_cee5e2356be79737e18519d78addf697.html)

    *   [boolean](http://help.scilab.org/docs/5.4.0/ja_JP/section_8b487f6dce31fb0d259e694eb038a228.html)

            *   [isBooleanType](http://help.scilab.org/docs/5.4.0/ja_JP/isBooleanType.html) — 检查是否它是一个布尔型的变量。
        *   [getScalarBoolean](http://help.scilab.org/docs/5.4.0/ja_JP/getScalarBoolean.html) — 从网关参数读取标量的布尔型数据。
        *   [createScalarBoolean](http://help.scilab.org/docs/5.4.0/ja_JP/createScalarBoolean.html) — Scilab 内存中创建标量的布尔变量。
        *   [booleanExample](http://help.scilab.org/docs/5.4.0/ja_JP/booleanExample.html) — 布尔值使用案例。

        *   [Boolean Sparse](http://help.scilab.org/docs/5.4.0/ja_JP/section_9528fc50b2dfbb890e38ffe30f792396.html)

            *   [isBooleanSparseType](http://help.scilab.org/docs/5.4.0/ja_JP/isBooleanSparseType.html) — 它是稀疏和一个布尔变量检查如果......
        *   [getAllocatedBooleanSparseMatrix](http://help.scilab.org/docs/5.4.0/ja_JP/getAllocatedBooleanSparseMatrix.html) — 得到稀疏矩阵 attributs。
        *   [freeAllocatedBooleanSparse](http://help.scilab.org/docs/5.4.0/ja_JP/freeAllocatedBooleanSparse.html) — GetAllocatedBooleanSparseMatrix 函数所分配的可用内存。
        *   [booleanSparseExample](http://help.scilab.org/docs/5.4.0/ja_JP/booleanSparseExample.html) — 布尔稀疏的用例。

        *   [Scilab Gateway API](http://help.scilab.org/docs/5.4.0/ja_JP/section_35dba248fab682a5eeaf230f1dcf0964.html)

            *   [How to](http://help.scilab.org/docs/5.4.0/ja_JP/section_dfbec616994039bd8e153ea3d0e671b9.html)

                    *   [CallingAScilabFunctionFromACInterface](http://help.scilab.org/docs/5.4.0/ja_JP/CallingAScilabFunctionFromACInterface.html) — 从 C 接口调用 scilab 函数 （宏）

                *   [CheckLhs](http://help.scilab.org/docs/5.4.0/ja_JP/CheckLhs.html) — C 宏哪些检查本中调用 Scilab 函数的输出参数的数目。 此函数已过时。
        *   [CheckRhs](http://help.scilab.org/docs/5.4.0/ja_JP/CheckRhs.html) — C 宏哪些检查本中调用 Scilab 函数的输入参数的数目。 此函数已过时。
        *   [Lhs](http://help.scilab.org/docs/5.4.0/ja_JP/Lhs.html) — 一个 C 网关函数，此函数提供的本中调用 Scilab 函数的输出参数的数目是过时的。
        *   [LhsVar](http://help.scilab.org/docs/5.4.0/ja_JP/LhsVar.html) — C 网关功能，指定哪些参数创建内部的 C 网关将返回作为输出参数到 Scilab。 此函数已过时。
        *   [Rhs](http://help.scilab.org/docs/5.4.0/ja_JP/Rhs.html) — 一个 C 网关函数，此函数提供本中调用 Scilab 函数的输入参数的数目是过时的。
        *   [Scierror](http://help.scilab.org/docs/5.4.0/ja_JP/Scierror.html) — C 网关功能，向用户 （作为 printf 函数相同浦飞尔) 显示一条错误消息，并返回一个整数值，指定错误级别
        *   [sci_types](http://help.scilab.org/docs/5.4.0/ja_JP/sci_types.html) — C 枚举，它定义了可用于一个变量的类型
        *   [sciprint](http://help.scilab.org/docs/5.4.0/ja_JP/sciprint.html) — C 网关功能显示标准的消息给用户 （在 C 函数中的 printf 作为同一浦飞尔)

        *   [double](http://help.scilab.org/docs/5.4.0/ja_JP/section_716eb11475497ac097dbd015adb39545.html)

            *   [isDoubleType](http://help.scilab.org/docs/5.4.0/ja_JP/isDoubleType.html) — 检查是否它是一个双变量。
        *   [getScalarDouble](http://help.scilab.org/docs/5.4.0/ja_JP/getScalarDouble.html) — 得到的标量双变量。
        *   [getScalarComplexDouble](http://help.scilab.org/docs/5.4.0/ja_JP/getScalarComplexDouble.html) — 得到的标量的复杂双变量。
        *   [createScalarDouble](http://help.scilab.org/docs/5.4.0/ja_JP/createScalarDouble.html) — Scilab 内存中创建一个标量双精度型。
        *   [createScalarComplexDouble](http://help.scilab.org/docs/5.4.0/ja_JP/createScalarComplexDouble.html) — Scilab 内存中创建标量的复杂双。
        *   [doubleExample](http://help.scilab.org/docs/5.4.0/ja_JP/doubleExample.html) — 双用例。

        *   [integer](http://help.scilab.org/docs/5.4.0/ja_JP/section_ae29f09e94041377c5ad83b5059479d2.html)

            *   [isIntegerType](http://help.scilab.org/docs/5.4.0/ja_JP/isIntegerType.html) — 检查是否它是一个双变量。
        *   [getScalarInteger8](http://help.scilab.org/docs/5.4.0/ja_JP/getScalarInteger8.html) — 获取标量整数变量。
        *   [createScalarInteger8](http://help.scilab.org/docs/5.4.0/ja_JP/createScalarInteger8.html) — 创建标量整数变量。
        *   [integerExample](http://help.scilab.org/docs/5.4.0/ja_JP/integerExample.html) — 整数的用例。

        *   [List manipulation](http://help.scilab.org/docs/5.4.0/ja_JP/section_281790c19f32a08419bf50d192e51020.html)

            *   [isListType](http://help.scilab.org/docs/5.4.0/ja_JP/isListType.html) — 请检查是否列表、 mlist、 tlist 变量。
        *   [list_boolean_reading_API](http://help.scilab.org/docs/5.4.0/ja_JP/list_boolean_reading_API.html) — 如何读取的 boolean 类型的值列表中的一个矩阵。
        *   [list_boolean_writing_API](http://help.scilab.org/docs/5.4.0/ja_JP/list_boolean_writing_API.html) — 如何在列表中添加一个 boolean 类型的值的矩阵。
        *   [list_bsparse_reading_API](http://help.scilab.org/docs/5.4.0/ja_JP/list_bsparse_reading_API.html) — 如何读取一个布尔值，稀疏的列表中。
        *   [list_bsparse_writing_API](http://help.scilab.org/docs/5.4.0/ja_JP/list_bsparse_writing_API.html) — 如何在列表中添加一个 boolean 类型的值的稀疏矩阵。
        *   [list_createlist_API](http://help.scilab.org/docs/5.4.0/ja_JP/list_createlist_API.html) — 如何获取 Scilab 内存中创建一个列表。
        *   [list_double_reading_API](http://help.scilab.org/docs/5.4.0/ja_JP/list_double_reading_API.html) — 如何读取一个矩阵的双列表中。
        *   [list_double_writing_API](http://help.scilab.org/docs/5.4.0/ja_JP/list_double_writing_API.html) — 如何添加矩阵的双列表中。
        *   [list_getlistitemaddress_API](http://help.scilab.org/docs/5.4.0/ja_JP/list_getlistitemaddress_API.html) — 如何获取列表子的地址。
        *   [list_getlistitemnumber_API](http://help.scilab.org/docs/5.4.0/ja_JP/list_getlistitemnumber_API.html) — 如何获取列表 （列表、 tlist、 mlist) 中的项目数。
        *   [list_integer_reading_API](http://help.scilab.org/docs/5.4.0/ja_JP/list_integer_reading_API.html) — 如何读取整数列表中的矩阵。
        *   [list_integer_writing_API](http://help.scilab.org/docs/5.4.0/ja_JP/list_integer_writing_API.html) — 如何在列表中添加矩阵的整数。
        *   [list_pointer_reading_API](http://help.scilab.org/docs/5.4.0/ja_JP/list_pointer_reading_API.html) — 如何读取列表中的指针。
        *   [list_pointer_writing_API](http://help.scilab.org/docs/5.4.0/ja_JP/list_pointer_writing_API.html) — 如何在列表中添加指针。
        *   [list_poly_reading_API](http://help.scilab.org/docs/5.4.0/ja_JP/list_poly_reading_API.html) — 如何读取列表中的多项式矩阵。
        *   [list_poly_writing_API](http://help.scilab.org/docs/5.4.0/ja_JP/list_poly_writing_API.html) — 如何在列表中添加的多项式矩阵。
        *   [list_sparse_reading_API](http://help.scilab.org/docs/5.4.0/ja_JP/list_sparse_reading_API.html) — 如何读取稀疏的列表中。
        *   [list_sparse_writing_API](http://help.scilab.org/docs/5.4.0/ja_JP/list_sparse_writing_API.html) — 如何在列表中添加稀疏矩阵。
        *   [list_string_reading_API](http://help.scilab.org/docs/5.4.0/ja_JP/list_string_reading_API.html) — 如何读取字符串列表中的矩阵。
        *   [list_string_writing_API](http://help.scilab.org/docs/5.4.0/ja_JP/list_string_writing_API.html) — 如何在列表中添加矩阵的字符串。

        *   [Low level functions](http://help.scilab.org/docs/5.4.0/ja_JP/section_7e77120ee5d903b802fb68addca649e0.html)

            *   [AssignOutputVariable](http://help.scilab.org/docs/5.4.0/ja_JP/AssignOutputVariable.html) — C 网关功能，指定哪些参数创建内部的 C 网关将返回作为输出参数到 Scilab。
        *   [CallOverloadFunction](http://help.scilab.org/docs/5.4.0/ja_JP/CallOverloadFunction.html) — C 网关功能使用调用重载函数或宏
        *   [CheckInputArgument](http://help.scilab.org/docs/5.4.0/ja_JP/CheckInputArgument.html) — C 函数，检查本中调用 Scilab 函数的输入参数的数目。
        *   [CheckOutputArgument](http://help.scilab.org/docs/5.4.0/ja_JP/CheckOutputArgument.html) — C 函数，检查本中调用 Scilab 函数的输出参数的数目。
        *   [ReturnArguments](http://help.scilab.org/docs/5.4.0/ja_JP/ReturnArguments.html) — 一个 C 网关函数，返回的各种变量。
        *   [boolean_reading_API](http://help.scilab.org/docs/5.4.0/ja_JP/boolean_reading_API.html) — 如何读取一个布尔值的矩阵。
        *   [boolean_writing_API](http://help.scilab.org/docs/5.4.0/ja_JP/boolean_writing_API.html) — 如何写的布尔值的矩阵。
        *   [bsparse_reading_API](http://help.scilab.org/docs/5.4.0/ja_JP/bsparse_reading_API.html) — 如何读取一个布尔值，稀疏的网关。
        *   [bsparse_writing_API](http://help.scilab.org/docs/5.4.0/ja_JP/bsparse_writing_API.html) — 如何在一个网关添加布尔稀疏矩阵。
        *   [check_matrix_dimension](http://help.scilab.org/docs/5.4.0/ja_JP/check_matrix_dimension.html) — 检查变量的维度 C 网关职能。
        *   [Common_getvaraddr_API](http://help.scilab.org/docs/5.4.0/ja_JP/Common_getvaraddr_API.html) — 如何获取参数或变量的地址在一个网关。
        *   [Common_getvardimension_API](http://help.scilab.org/docs/5.4.0/ja_JP/Common_getvardimension_API.html) — 如何获取的参数或变量作为矩阵存储尺寸。
        *   [Common_getvartype_API](http://help.scilab.org/docs/5.4.0/ja_JP/Common_getvartype_API.html) — 如何获取类型的参数或变量内的网关。
        *   [Common_iscomplex_API](http://help.scilab.org/docs/5.4.0/ja_JP/Common_iscomplex_API.html) — 如何获取的参数或变量的复杂性。
        *   [Common_isvarmatrixtype_API](http://help.scilab.org/docs/5.4.0/ja_JP/Common_isvarmatrixtype_API.html) — 如何知道是否一个参数或变量存储为一个矩阵。
        *   [deleteNamedVariable](http://help.scilab.org/docs/5.4.0/ja_JP/deleteNamedVariable.html) — C 网关函数中用来从名称中删除变量
        *   [Double_management_reading_API](http://help.scilab.org/docs/5.4.0/ja_JP/Double_management_reading_API.html) — 如何读取的双网关在矩阵。
        *   [Double_management_writing_API](http://help.scilab.org/docs/5.4.0/ja_JP/Double_management_writing_API.html) — 如何写的双打矩阵中的网关。
        *   [getNbInputArgument](http://help.scilab.org/docs/5.4.0/ja_JP/getNbInputArgument.html) — C 网关功能，提供本中调用 Scilab 函数的输入参数的数目
        *   [getNbOutputArgument](http://help.scilab.org/docs/5.4.0/ja_JP/getNbOutputArgument.html) — C 网关功能，它提供的本中调用 Scilab 函数的输出参数的数目
        *   [int_getmatrixofintegerprecision_API](http://help.scilab.org/docs/5.4.0/ja_JP/int_getmatrixofintegerprecision_API.html) — 如何获取整数矩阵的精度。
        *   [Integer_management_reading_API](http://help.scilab.org/docs/5.4.0/ja_JP/Integer_management_reading_API.html) — 如何读取整数中网关的矩阵。
        *   [Integer_management_writing_API](http://help.scilab.org/docs/5.4.0/ja_JP/Integer_management_writing_API.html) — 如何写的整数矩阵中的网关。
        *   [Pointer_reading_API](http://help.scilab.org/docs/5.4.0/ja_JP/Pointer_reading_API.html) — 如何读取指针在一个网关。
        *   [Pointer_writing_API](http://help.scilab.org/docs/5.4.0/ja_JP/Pointer_writing_API.html) — 如何写指针在一个网关。
        *   [poly_getpolyvariablename_API](http://help.scilab.org/docs/5.4.0/ja_JP/poly_getpolyvariablename_API.html) — 如何获取的符号的变量名称。
        *   [Polynomial_management_reading_API](http://help.scilab.org/docs/5.4.0/ja_JP/Polynomial_management_reading_API.html) — 如何读取的矩阵多项式的网关。
        *   [Polynomial_management_writing_API](http://help.scilab.org/docs/5.4.0/ja_JP/Polynomial_management_writing_API.html) — 如何写的多项式矩阵中的网关。
        *   [Sparse_management_reading_API](http://help.scilab.org/docs/5.4.0/ja_JP/Sparse_management_reading_API.html) — 如何读取中网关的稀疏矩阵。
        *   [Sparse_management_writing_API](http://help.scilab.org/docs/5.4.0/ja_JP/Sparse_management_writing_API.html) — 如何写稀疏矩阵中的网关。
        *   [String_management_reading_API](http://help.scilab.org/docs/5.4.0/ja_JP/String_management_reading_API.html) — 如何读取字符串中网关的矩阵。
        *   [String_management_writing_API](http://help.scilab.org/docs/5.4.0/ja_JP/String_management_writing_API.html) — 如何在一个网关写字符串的矩阵。

        *   [polynomial](http://help.scilab.org/docs/5.4.0/ja_JP/section_8d90340fb1ee1e77460ea01dbc2ded9f.html)

            *   [isPolyType](http://help.scilab.org/docs/5.4.0/ja_JP/isPolyType.html) — 检查是否它是一个多项式的变量。
        *   [getAllocatedSinglePoly](http://help.scilab.org/docs/5.4.0/ja_JP/getAllocatedSinglePoly.html) — 获取单个多项式变量。
        *   [getAllocatedSingleComplexPoly](http://help.scilab.org/docs/5.4.0/ja_JP/getAllocatedSingleComplexPoly.html) — 获取单个复杂多项式变量。
        *   [getAllocatedMatrixOfPoly](http://help.scilab.org/docs/5.4.0/ja_JP/getAllocatedMatrixOfPoly.html) — 得到多项式变量的矩阵。
        *   [getAllocatedMatrixOfComplexPoly](http://help.scilab.org/docs/5.4.0/ja_JP/getAllocatedMatrixOfComplexPoly.html) — 获取复杂多项式变量的矩阵。
        *   [freeAllocatedSinglePoly](http://help.scilab.org/docs/5.4.0/ja_JP/freeAllocatedSinglePoly.html) — GetAllocatedSinglePoly 函数所分配的可用内存。
        *   [freeAllocatedSingleComplexPoly](http://help.scilab.org/docs/5.4.0/ja_JP/freeAllocatedSingleComplexPoly.html) — GetAllocatedSingleComplexPoly 函数所分配的可用内存。
        *   [freeAllocatedMatrixOfPoly](http://help.scilab.org/docs/5.4.0/ja_JP/freeAllocatedMatrixOfPoly.html) — GetAllocatedSinglePoly 函数所分配的可用内存。
        *   [freeAllocatedMatrixOfComplexPoly](http://help.scilab.org/docs/5.4.0/ja_JP/freeAllocatedMatrixOfComplexPoly.html) — GetAllocatedSinglePoly 函数所分配的可用内存。
        *   [polyExample](http://help.scilab.org/docs/5.4.0/ja_JP/polyExample.html) — Polynom 使用案例。

        *   [sparse](http://help.scilab.org/docs/5.4.0/ja_JP/section_e256957ca787af977ccdc67af24e7987.html)

            *   [isSparseType](http://help.scilab.org/docs/5.4.0/ja_JP/isSparseType.html) — 检查是否是一个稀疏的变量。
        *   [getAllocatedSparseMatrix](http://help.scilab.org/docs/5.4.0/ja_JP/getAllocatedSparseMatrix.html) — 得到稀疏矩阵变量。
        *   [getAllocatedComplexSparseMatrix](http://help.scilab.org/docs/5.4.0/ja_JP/getAllocatedComplexSparseMatrix.html) — 获取复杂稀疏矩阵变量。
        *   [freeAllocatedSparseMatrix](http://help.scilab.org/docs/5.4.0/ja_JP/freeAllocatedSparseMatrix.html) — GetAllocatedSparseMatrix 函数所分配的可用内存。
        *   [freeAllocatedComplexSparseMatrix](http://help.scilab.org/docs/5.4.0/ja_JP/freeAllocatedComplexSparseMatrix.html) — GetAllocatedComplexSparseMatrix 函数所分配的可用内存。
        *   [sparseExample](http://help.scilab.org/docs/5.4.0/ja_JP/sparseExample.html) — 稀疏的用例。

        *   [string](http://help.scilab.org/docs/5.4.0/ja_JP/section_56d380c514ce4270f3a78e081a99d248.html)

            *   [isStringType](http://help.scilab.org/docs/5.4.0/ja_JP/isStringType.html) — 检查是否是一个字符串变量。
        *   [getAllocatedSingleString](http://help.scilab.org/docs/5.4.0/ja_JP/getAllocatedSingleString.html) — 获取一个字符串变量。
        *   [getAllocatedMatrixOfString](http://help.scilab.org/docs/5.4.0/ja_JP/getAllocatedMatrixOfString.html) — 获取一个字符串变量的矩阵。
        *   [createSingleString](http://help.scilab.org/docs/5.4.0/ja_JP/createSingleString.html) — 创建一个单一的字符串变量。
        *   [freeAllocatedSingleString](http://help.scilab.org/docs/5.4.0/ja_JP/freeAllocatedSingleString.html) — GetAllocatedSinglePoly 函数所分配的可用内存。
        *   [freeAllocatedMatrixOfString](http://help.scilab.org/docs/5.4.0/ja_JP/freeAllocatedMatrixOfString.html) — FreeAllocatedMatrixOfString 函数所分配的可用内存。
        *   [stringExample](http://help.scilab.org/docs/5.4.0/ja_JP/stringExample.html) — 字符串使用案例。

        *   [api_scilab](http://help.scilab.org/docs/5.4.0/ja_JP/api_scilab.html) — api_scilab 是要读/写数据从到 Scilab 内存的 Scilab 接口
    *   [api_scilab_getting_started](http://help.scilab.org/docs/5.4.0/ja_JP/api_scilab_getting_started.html) — 如何加载 a C、 C 或 fortran Scilab 引擎作为一个新的函数中的代码

*   调用scilabAPI[call_scilab API](http://help.scilab.org/docs/5.4.0/ja_JP/section_8843de3c2c20adacaed1d55195fb1d34.html)

    *   [BooleanManagement_callscilab](http://help.scilab.org/docs/5.4.0/ja_JP/BooleanManagement_callscilab.html) — 如何管理 Scilab 的布尔值，读取和写入进程使用 call_scilab 和 api_scilab
    *   [ComplexManagement_callscilab](http://help.scilab.org/docs/5.4.0/ja_JP/ComplexManagement_callscilab.html) — 如何管理 Scilab 的复变量读取和写入进程使用 call_scilab
    *   [DisableInteractiveMode](http://help.scilab.org/docs/5.4.0/ja_JP/DisableInteractiveMode.html) — 禁用某些功能 (策划、 创作的 gui，Tcl/Tk，......) 和叶只有计算引擎
    *   [DoubleManagement_callscilab](http://help.scilab.org/docs/5.4.0/ja_JP/DoubleManagement_callscilab.html) — 如何管理 Scilab 的变量中读取和写入进程使用 call_scilab 和 api_scilab
    *   [GetLastJob](http://help.scilab.org/docs/5.4.0/ja_JP/GetLastJob.html) — 返回发送到 Scilab 引擎的最新作业
    *   [ScilabHaveAGraph](http://help.scilab.org/docs/5.4.0/ja_JP/ScilabHaveAGraph.html) — 检查任何 Scilab 图形是否已打开。
    *   [SendScilabJob](http://help.scilab.org/docs/5.4.0/ja_JP/SendScilabJob.html) — 从 c/c 代码 (call_scilab) 发送 Scilab 任务
    *   [SendScilabJobs](http://help.scilab.org/docs/5.4.0/ja_JP/SendScilabJobs.html) — 从 c/c 代码 (call_scilab) 发送 Scilab 任务
    *   [StartScilab](http://help.scilab.org/docs/5.4.0/ja_JP/StartScilab.html) — 初始化和启动 Scilab 引擎中调用 Scilab
    *   [StringManagement_callscilab](http://help.scilab.org/docs/5.4.0/ja_JP/StringManagement_callscilab.html) — 如何管理 Scilab 的字符串读取和写入进程使用 call_scilab 和 api_scilab
    *   [TerminateScilab](http://help.scilab.org/docs/5.4.0/ja_JP/TerminateScilab.html) — 停止和终止中调用 Scilab Scilab 引擎
    *   [call_scilab](http://help.scilab.org/docs/5.4.0/ja_JP/call_scilab.html) — call_scilab 是一个界面，提供了从 c/c 代码中调用 Scilab 引擎的能力
    *   [compile_and_run_call_scilab](http://help.scilab.org/docs/5.4.0/ja_JP/compile_and_run_call_scilab.html) — 如何编译本机应用程序的基础上或使用 Scilab
    *   [fromc](http://help.scilab.org/docs/5.4.0/ja_JP/fromc.html) — 检查是否当前 Scilab 从外部 C 程序调用 （由 StartScilab)。
    *   [fromjava](http://help.scilab.org/docs/5.4.0/ja_JP/fromjava.html) — 检查是否当前 Scilab 从 javasci 调用

*   Java接口[Java Interface](http://help.scilab.org/docs/5.4.0/ja_JP/section_dca2d856b03ac6ecc1570b33ccb6bf5f.html)

    *   [compile_and_run_javasci_v2](http://help.scilab.org/docs/5.4.0/ja_JP/compile_and_run_javasci_v2.html) — 如何编译 Java 应用程序中使用 Javasci v2
    *   [javasci](http://help.scilab.org/docs/5.4.0/ja_JP/javasci.html) — 从 Java 应用程序中调用 Scilab 引擎
    *   [javasci_faq_v2](http://help.scilab.org/docs/5.4.0/ja_JP/javasci_faq_v2.html) — Javasci v2 常见问题
    *   [javasci_v1_limitations](http://help.scilab.org/docs/5.4.0/ja_JP/javasci_v1_limitations.html) — 为什么 javasci v1 现已被否决？
    *   [javasci_step_by_step](http://help.scilab.org/docs/5.4.0/ja_JP/javasci_step_by_step.html) — 如何编写应用程序，基于 javasci v2

*   [Intersci](http://help.scilab.org/docs/5.4.0/ja_JP/section_b5163beab78f5a26d2d0341ddc7cbe2a.html)

    *   [intersci](http://help.scilab.org/docs/5.4.0/ja_JP/intersci.html) — Scilab 到接口 C 或 Fortran 函数与 scilab 的工具。 不推荐使用： 请使用SWIG

*   Windows 系统工具[Windows tools](http://help.scilab.org/docs/5.4.0/ja_JP/section_845186cafe6299fdd8fbc1a5d49027b8.html)

    *   [dos](http://help.scilab.org/docs/5.4.0/ja_JP/dos.html) — (Cmd) 执行 shell 命令 （仅限 Windows）
    *   [chartooem](http://help.scilab.org/docs/5.4.0/ja_JP/chartooem.html) — 字符串转换的 OEM 定义的字符集 （仅 Windows）
    *   [consolebox](http://help.scilab.org/docs/5.4.0/ja_JP/consolebox.html) — 显示或隐藏控制台框 (Windows)
    *   [createGUID](http://help.scilab.org/docs/5.4.0/ja_JP/createGUID.html) — 创建一个 GUID （仅 Windows）
    *   [findfileassociation](http://help.scilab.org/docs/5.4.0/ja_JP/findfileassociation.html) — 搜索和检索文件协会相关字符串从注册表 （仅 Windows）
    *   [getsystemmetrics](http://help.scilab.org/docs/5.4.0/ja_JP/getsystemmetrics.html) — 检索指定的系统公制或配置设置系统 （仅限 Windows）
    *   [istssession](http://help.scilab.org/docs/5.4.0/ja_JP/istssession.html) — 确定是否 scilab 启动从 ms 终端服务会话 （仅 Windows）
    *   [mcisendstring](http://help.scilab.org/docs/5.4.0/ja_JP/mcisendstring.html) — 将命令字符串发送到 MCI 设备 （仅 Windows）
    *   [oemtochar](http://help.scilab.org/docs/5.4.0/ja_JP/oemtochar.html) — （仅限 Windows） 转换为 ANSI 字符串到 OEM 定义字符集中的字符串
    *   [powershell](http://help.scilab.org/docs/5.4.0/ja_JP/powershell.html) — (powershell） 执行命令外壳程序 （仅 Windows）
    *   [win64](http://help.scilab.org/docs/5.4.0/ja_JP/win64.html) — 确定是否 Windows x64 版本的 Scilab （仅 Windows）
    *   [winopen](http://help.scilab.org/docs/5.4.0/ja_JP/winopen.html) — 打开的文件在适当的应用程序 （仅 Windows）
    *   [winqueryreg](http://help.scilab.org/docs/5.4.0/ja_JP/winqueryreg.html) — 从 Microsoft Windows 注册表 （仅 Windows） 获取项目