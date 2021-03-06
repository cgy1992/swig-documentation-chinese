# 2.2 为什么使用SWIG

正如前面阐述的，SWIG主要用于简化其他语言与C/C++语言的集成。为什么大家要这样做呢？为了回答这个问题，列出C/C++语言的长处是必要的：

+ 对编写编程库的极好支持
+ 高性能(数字、数据、图像处理等)
+ 系统编程与系统集成
+ 大的用户基础与软件基础

C/C++语言的问题：

+ 编写用户界面很让人痛苦(比如，使用MFC、X11、GTK或其他的库)
+ 测试起来浪费时间(the compile/debug cycle)
+ 不重新编译就不太容易重新配置或自定义
+ 模块化很棘手
+ 安全问题（例如缓冲区溢出）

为了解决这些限制，许多程序员认为：应该使用不同的编程语言来完成不同的任务。例如，使用像Python或Tcl这样的脚本语言，编写图形用户界面可能非常容易（考数以百万计的程序员使用了像VisualBasic这样的语言就是证据）。交互式解释器也可以作为有用的调试和测试工具。其他语言如java可以大大简化编写分布式计算软件的任务。关键是不同的编程语言提供了不同的优点和缺点。而且，任何编程都不可能十全十美。因此，通过将语言结合在一起，您可以利用每种语言的最佳特性，并大大简化软件开发的某些方面。

站在C/C++的方面来说，很多人使用SWIG时因为他们可以打破传统的单一C语言编程模型，这样的模型表现如下：

+ 一组有用的函数和变量的集合
+ 从main()启动程序
+ 启动用户界面要做一大堆的工作（一般人都不想再这么干了）

将C／C集成到更高级的语言中，通常会带来更模块化的设计、更少的代码、更好的灵活性，从而提高程序员的生产力。

SWIG尽量让C/C++程序的集成变得更轻松。这使您能够专注于底层的C程序并使用高级语言接口，而不用关注语言间集成等繁琐的工作。同时，SWIG认为所有的应用程序是不同的。因此，它提供了各种各样的定制功能，使您几乎可以改变语言绑定的每一个方面。这就是为什么SWIG有这么大的一个用户手册的主要原因。  :happy:  