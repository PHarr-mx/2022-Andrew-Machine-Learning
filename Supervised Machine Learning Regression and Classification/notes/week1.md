# 机器学习的定义

一种不需要明确的办成就能让计算机学习的研究领域。

机器学习算法分

- Supervised learning 有监督机器学习
- Unsupervised learning 无监督机器学习

除此之外还有一种 Reinforcement learning 强化学习

# Supervised Learning 监督学习

给出学习算法示例，即对于输入x和输出标签y。最终的结果是给定任意输入x，给出合适的预期标签y。

## Regression 回归

![image-20230414110657511](https://s2.loli.net/2023/04/14/FMkdDfrY4a6vxiB.png)

这是一个经典的回归模型，他的主要任务是预测数字，回归模型的预测结果有无限种可能性。回归模型拟合的结果不一定是直线，比如这里曲线的拟合是更加准确的。

## Classification 分类

![image-20230414112452524](https://s2.loli.net/2023/04/14/mT9MLeCbYvVaESQ.png)

这是一个分类算法，他主要是把肿瘤分成良性和恶性两种。

![image-20230414113718197](https://s2.loli.net/2023/04/14/JFN3y9jlZEg6iBz.png)

由此可以看出，分类算法的预测结果不一定是数字，并且分类算法的预测结果也是在一给小范围的集合当中。

# Unsupervised Learning 无监督学习

Find something interesting in unlabeled data. 在无标签的数据中找到有趣的东西。

## Clustering 聚类

![image-20230419095408272](https://s2.loli.net/2023/04/19/xftBCAYLojqiUab.png)

可以看到上面的文章标题中都出现了panda、twin、zoo 三个共同的词，所以谷歌新闻把这些文章判定为了同一类的文章。值得注意的是，算法工程师并没有指定要把这三个词归为一类，完全是算法自己判定的。

![image-20230419100212313](https://s2.loli.net/2023/04/19/hsOctzSDMLvEeNa.png)

这又是一个聚类算法的例子，上图是一共DNA图谱，每一列表示一共人的基性性状，每一行表示一种基因，不同的颜色表示基因的不同性状。可以看到聚类算法把这些人按照基因分成了三类，但实际上我们并没有规定type1,type2,type3所表现的性状应该是什么，一切都是由算法决定的。

Which is a type  of unsupervised learning algorithm,takes data without labels and tries to  automatically group them into clusters.

这是一种无监督的学习算法，在没有标签的情况下获取数据，并试图将它们自动归类为集群。

无监督学习的一个准确的定义：**Data only comes with inputs x ,but not output labels y. Algorithm has to find structure in the data.**

三种常见的无监督学习

1. Clustering: Group similar data points together.
2. Anomaly detection: Find unusual data points.
3. Dimensionality reduction: Compress data using fewer numbers.

# Linear Regression Model 线性回归模型

在机器学习中常用的数据集表示方法有两种

![image-20230428152153266](https://s2.loli.net/2023/04/28/zF1yewkI9nbhOv6.png)

Data table 中每一行都对应了坐标图中的一个点

下面规定了一些符号的表示方法

![image-20230428152303830](https://s2.loli.net/2023/04/28/UhVyo2dHKuZ38bg.png)

![image-20230428152810935](https://s2.loli.net/2023/04/28/Z35SnG76bNXDJga.png)

我们根据training set 可以得到 function 记作$f$，$f(x)=\hat{y}$，这里的$\hat y$ 读作`y-hat`表示的是预测值，而$y$表示真实值，也就是target。

在线性回归中的重点就是如何用数学公式表示$f$

