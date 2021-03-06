# LSTM参数个数计算
个人认为明白如何计算一个网络的参数个数，对于理解一个网络的流程特别重要。

[参考链接](https://zhuanlan.zhihu.com/p/39262960)


[这个链接里面直接有公式](https://www.cnblogs.com/wdmx/p/9284037.html)

首先声明：

参数个数与steps无关

h_t 的维度与 c_t 相同

两个门来控制状态 ，一个门来控制状态 对输出的影响。

有四个交互的层，也就是拥有四组【w,b】参数；所以 总参数个数= (w的元素个数 + b的元素个数)*4 总参数个数的元素个数的元素个数

向量经过激活函数后，仍是一个向量：对向量中的每一个元素分别操作


重点：计算出 w,b 的维度，就计算出参数个数了

![](https://pic4.zhimg.com/80/v2-558af6af92912390c3f1371b9ac0469f_hd.jpg)

从上图中可以看出，每个交互的层的操作大致是一样的，主要都是：

> w * []+b

然后再经过激活函数，之后再与状态 c 作用，与参数有关的就是 w*[]+b 。



因为输入输出向量的维度都是我们提前规定好的，假设维度是：

> x:2024 * 1,h维度=c维度=50 * 1



所以，根据公式：已知



> W*[h;x] + b= 输出维度

> W*[(2024+50)*1] + 50 * 1 = 50 * 1

> W [50*2074]

所以，可以根据维度倒推出维度：



> w: 50*2074， b:50*1



四组【w,b】,所以总参数：

> 4*（50*2074+50）= 415000
