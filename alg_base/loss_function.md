# 损失函数 loss function

### 基本概念
学习算法的目标是找到最好的参数，然而怎么衡量这个最好的问题？答案是**损失函数（loss function)**。

数据标签（label）与预测结果（predict）之间差距叫做损失，衡量损失的函数叫做损失函数。

在有监督学习（supervised learning）中，不同模型根据各自不同的目标，都会定义有各自的损失函数，例如：
* 线性回归（linear regression）中的平方损失函数；
* 逻辑回归（logistic regression）中的log损失函数；
* svm算法中定义的hinge损失函数；

*有很多paper就是对损失函数做优化。*

# 常见的损失函数

机器学习或者统计机器学习常见的损失函数如下：

1.0-1损失函数 （0-1 loss function）

L(Y,f(X))={1,Y ≠ f(X)
           0,Y = f(X)

2.平方损失函数（quadratic loss function)

L(Y,f(X))=(Y−f(x))2

3.绝对值损失函数(absolute loss function)

L(Y,f(x))=|Y−f(X)|

4.对数损失函数（logarithmic loss function) 或对数似然损失函数(log-likehood loss function)

L(Y,P(Y|X))=−logP(Y|X)
逻辑回归中，采用的则是对数损失函数。如果损失函数越小，表示模型越好。

### eg.
在线性回归中，model定义：

![](https://github.com/bobkentt/Learning-machine-from-scratch-pic/blob/master/alg_base/pic/20170521165243.png)

在线性回归model中，损失函数是取predict value与label value的方差，定义如下：

![](https://github.com/bobkentt/Learning-machine-from-scratch-pic/blob/master/alg_base/pic/20170521165348.png)

在参数是一元的情况下：

![](https://github.com/bobkentt/Learning-machine-from-scratch-pic/blob/master/alg_base/pic/20170521171921.png)

在多元的情况下：

![](https://github.com/bobkentt/Learning-machine-from-scratch-pic/blob/master/alg_base/pic/20170521171944.png)

平方loss在linear regression的情况下是一个凸函数，这意味着存在全局最优点，并且可能通过某些方法找到全局最优点。在deep learning中没有办法确保找到全局最优点，在工业上找到一个几乎是全局最优点的点，在工业上可以用就行了。

### 线性回归与梯度下降GD
梯度下降算法的细节在：

[点此链接跳转到线性回归与梯度下降GD](https://github.com/bobkentt/Learning-machine-from-scratch-/blob/master/alg_base/ch1/gradient_descent.md)

除了梯度下降算法外，还有牛顿法，拟牛顿法等等优化算法。
