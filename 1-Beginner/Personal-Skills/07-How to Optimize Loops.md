# 如何优化循环

有时候你会遇到循环，或者递归函数，它们会花费很长的执行时间，可能是你的产品的瓶颈。在你尝试使循环变得快一点之前，花几分钟考虑是否有可能把它整个移除掉，有没有一个不同的算法？你可以在计算时做一些其他的事情吗？如果你不能找到一个方法去绕开它，你可以优化这个循环了。这是很简单的，move stuff out。最后，这不仅需要智慧而且需要理解每一种语句和表达式的开销。这里是一些建议：

- 删除浮点运算操作。
- 非必要时不要分配新的内存。
- 把常量都放在一起声明。
- 把 I/O 放在缓冲里做。
- 尽量不使用除法。
- 尽量不适用昂贵的类型转换。
- 移动指针而非重新计算索引。

这些操作的具体代价取决于你的具体系统。在一些系统中，编译器和硬件会为你做一些事情。但必须清楚，有效的代码比需要在特殊平台下理解的代码要好。

Next [如何处理I/O开销](08-How to Deal with IO Expense.md)
