# 3.各种分布

### 二项分布
![](https://github.com/bobkentt/Learning-machine-from-scratch-pic/blob/master/math_base/pic/10.png)

### 均匀分布

![](https://github.com/bobkentt/Learning-machine-from-scratch-pic/blob/master/math_base/pic/8.png)

### 泊松分布
*日常生活中，大量事件是有固定频率的。*


> *某医院平均每小时出生3个婴儿*
> *某公司平均每10分钟接到1个电话*
> *某超市平均每天销售4包xx牌奶粉*
> *某网站平均每分钟有2次访问*


它们的特点就是，我们可以预估这些事件的总数，但是没法知道具体的发生时间。已知平均每小时出生3个婴儿，请问下一个小时，会出生几个？

![](https://github.com/bobkentt/Learning-machine-from-scratch-pic/blob/master/math_base/pic/posong1.png)


### 指数分布
指数分布是事件的时间间隔的概率。下面这些都属于指数分布。


> 婴儿出生的时间间隔
> 来电的时间间隔
> 奶粉销售的时间间隔
> 网站访问的时间间隔

指数分布的公式可以从泊松分布推断出来。如果下一个婴儿要间隔时间 t ，就等同于 t 之内没有任何婴儿出生。

![](https://github.com/bobkentt/Learning-machine-from-scratch-pic/blob/master/math_base/pic/zhishu1.png)
![](https://github.com/bobkentt/Learning-machine-from-scratch-pic/blob/master/math_base/pic/zhishu2.png)

### 正态分布

![](https://github.com/bobkentt/Learning-machine-from-scratch-pic/blob/master/math_base/pic/zhengtai1.png)
![](https://github.com/bobkentt/Learning-machine-from-scratch-pic/blob/master/math_base/pic/zhengtai2.png)
![](https://github.com/bobkentt/Learning-machine-from-scratch-pic/blob/master/math_base/pic/zhengtai3.png)


### 几何分布
![](https://github.com/bobkentt/Learning-machine-from-scratch-pic/blob/master/math_base/pic/11.png)

### 总结
![](https://github.com/bobkentt/Learning-machine-from-scratch-pic/blob/master/math_base/pic/sum.png)

# 补充说明
1. 关于对泊松分布和指数分布的理解，强烈建议大家看一下下面这个博客；
[阮一峰的网络日志:泊松分布和指数分布：10分钟教程](http://www.ruanyifeng.com/blog/2015/06/poisson-distribution.html)  









2. Gamma分布在后续章节会有所涉及。
![](https://github.com/bobkentt/Learning-machine-from-scratch-pic/blob/master/math_base/gamma.png)
