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
$$此外，$$S$$中给定的向量$$\boldsymbol{p}$$和向量$$\boldsymbol{b} \in R^m$$最接近的充要条件是$$\boldsymbol{b} - \boldsymbol{p} \in S^\bot$$.



$$A^TA\boldsymbol{x} = A^T\boldsymbol{b}$$表示$$n\times n$$线性方程组称为**正规方程组(normal equations)**. 一般的正规方程组可能存在多个解；然面，若$$\boldsymbol{\widehat{x}}$$和$$\boldsymbol{\widehat{y}}$$均为解，则由于$$\boldsymbol{b}$$在$$R(A)$$中的投影$$\boldsymbol{p}$$是惟一的，故
$$
A\boldsymbol{\widehat{x}} = A\boldsymbol{\widehat{y}} = \boldsymbol{p}
$$
**定理** 若$$A$$是秩为n的$$m\times n$$矩阵，则正规方程组
$$
A^TA\boldsymbol{x} = A^T\boldsymbol{b}
$$有惟一解
$$
\boldsymbol{\widehat{x}} = (A^TA)^{-1}A^T\boldsymbol{b}
$$且$$\boldsymbol{\widehat{x}}$$为方程组$$A\boldsymbol{x} = \boldsymbol{b}$$惟一的最小二乘解.


