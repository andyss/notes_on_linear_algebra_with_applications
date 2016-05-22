### 5.3.1 超定方程组的最小二乘解

给定一个方程组$$A\boldsymbol{x} = \boldsymbol{b}$$，其中$$A$$为一个$$m\times n(m \gt n)$$矩阵，并且$$\boldsymbol{b} \in R^m$$，则对每一个$$\boldsymbol{x} \in R^n$$，可以构造一个**残差(residual)**
$$
r(\boldsymbol{x}) = \boldsymbol{b} - A\boldsymbol{x}
$$$$\boldsymbol{b}$$和$$A\boldsymbol{x}$$间的距离为
$$
\|\boldsymbol{b} - A\boldsymbol{x}\| = \|r(\boldsymbol{x})\|
$$我们希望寻找一个向量$$\boldsymbol{x} \in R^n$$，使得$$\|r(\boldsymbol{x})\|$$是最小的，最小化$$\|r(\boldsymbol{x})\|$$等价于最小化$$\|r(\boldsymbol{x})\|^2$$，达到最小值的向量$$\boldsymbol{\widehat{x}}$$称为方和组$$A\boldsymbol{x} = \boldsymbol{b}$$的**最小二乘解(least squares solution)**.


**定理** 令$$S$$为$$R^m$$的一个子空间，对每一个$$\boldsymbol{b} \in R^m$$，在$$S$$中均存在一个惟一的元素$$\boldsymbol{p}$$和$$\boldsymbol{b}$$最接近，即对任意$$\boldsymbol{y} \neq \boldsymbol{p}$$，有
$$
\|\boldsymbol{b} - \boldsymbol{y}\| \gt \|\boldsymbol{b} - \boldsymbol{p}\|
$$

