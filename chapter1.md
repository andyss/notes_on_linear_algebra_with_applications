### 1\.1 线性方程组

#### 1.1.1  $$m \times  n$$ 的线性方程组

形如
$$
a_1x_1 + a_2x_2 + \dotsb + a_nx_n = b
$$的方程称为含有$$n$$个未知量的**线性方程**. 含有m个线性方程称为$$m \times n$$的**线性方程组**.


若有序$$n$$元组$$(x_1, x_2, \dotsc, x_n)$$满足方程组中的所有方程，称之为方程组的**解**. 线性方程组的所有解的集合称为方程组的**解集**. 如果解集为空则称方程组是**不相容的(inconsistent)**，如果至少存在一个解，则称之为**相容的(consistent)**.

#### 1.1.2 等价方程组

*定义* 若两个含有相同变量的方程组具有相同的解集，则称它们是**等价的(equivalent)**.

有三种运算可以得到一个等价的方程组：

* 交换任意两个方程的顺序
* 任一方程两边同乘一个非零的实数
* 任一方程的倍数加到另一方程上


#### 1.1.3 $$n\times n$$方程组

*定义* 若方程组中，第$$k$$个方程的前$$k-1$$个变量的系数均为零，且$$x_k(k=1, \dotsc, n)$$的系数不为零，则称该方程组为**严格三解形的(strict triangular form)**.

> 例如  
$$
\begin{align}
3x_1 + 2x_2 + x_3 =1 \\
x_2 - x_3 = 2  \\
            2x_3 = 4 \\
\end{align}
$$


#### 1.1.4 系数矩阵

我们可以将$$m \times n$$的方程组简化为一个$$m \times n$$的矩阵. 称之为**系数矩阵(coefficient matrix)**.

如果将系数矩阵右侧添加一列方程组的右端项，可得到一个新的矩阵，称之为**增广矩阵(augmented matrix)**.

> 例如  
$$
\left[
    \begin{array}{ccc|c}
      a_{11} & \dotsc & a_{1n} & b_1 \\
      \vdots &        &        & \vdots \\
      a_{m1} & \dotsc & a_{mn} & b_m
    \end{array}
\right] \tag{7}
$$


#### 1.1.5 初等行运算

* 交换两行
* 以非零实数乘以某行
* 将某行替换为它与其他行倍数的和


### 1.2 行阶梯形

*定义* 若一个矩阵满足
* 每一非零行中的第一个非零元为1
* 第$$k$$行的元不全为零时，第$$k+1$$行首变量之前零的个数多于第$$k$$行首变量之前的零的个数
* 所有元素均为零的行必在不全为零的行之后

则称其为**行阶梯矩阵(row echelon form)**.


*定义* 若一个线性方程组中方程的个数多于未知量的个数，则称其为**超定的(overdetermined)**.

*定义* 若一个线性方程组中方程的个数少于未知量的个数，则称其为**亚定的(underdeterminded)**.

*定义* 若一个矩阵满足
* 矩阵是行阶梯形的
* 每一行的第一个非零元是该列惟一的非零元

则称其为**行最简形(reduced row echelon form)**.

*定义* 如果线性方程组的右端若项全为零，则称其为**齐次的(homogeneous)**. 即$$A\boldsymbol{x} = 0$$的时候.


### 1.3 矩阵算术

我们一般用$$\overrightarrow{x}$$表示**行向量(row vector)**，用加粗的小字母$$\boldsymbol{x}$$表示**列向量(column vector)**. 我们一般将列向量简称为向量.

**相等**

*定义* 若两个$$m \times n$$矩阵$$A$$和$$B$$对任一$$i$$和$$j$$均满足$$a_{ij} = b_{ij}$$，则称它们**相等(equal)**.

**标量乘法**

*定义* 若$$A$$为$$m \times n$$的矩阵，且$$\alpha$$为一标量，则$$\alpha A$$为一个$$m \times n$$的矩阵，其$$(i, j)$$元素为$$\alpha a_{ij}$$.

**矩阵加法**

*定义* 设$$A = (a_{ij})$$及$$B = (b_{ij})$$都是$$m \times n$$的矩阵，则它们的**和(sum)**$$A + B$$也为一个$$m \times n$$的矩阵，对每一个有序对$$(i, j)$$，它的(i, j)的元素为$$a_{ij} + b_{ij}$$.

**线性组合**

*定义* 若$$\boldsymbol{a_1, a_2, \dotsc, a_n}$$，为$$R^m$$中的向量，且$$c_1, c_2, \dotsc, c_n$$为标题，则和式
$$
c_1\boldsymbol{a_1} + c_2\boldsymbol{a_2} + \dotsb + c_n\boldsymbol{a_n}
$$
称为向量$$\boldsymbol{a_1, a_2, \dotsc, a_n}$$的一个**线性组合(linear combination)**.

** 矩阵乘法**

*定义* 若$$A = (a_{ij})$$为一个$$m \times n$$的矩阵，且$$B = (b_{ij})$$为一个$$n \times r$$的矩阵，则乘积$$AB = C = (c_{ij})$$为一个$$m \times r$$的矩阵，它的元素定义为
$$
c_{ij} = \boldsymbol{\overrightarrow{a_i}b_j} = \sum_{k = 1}^n a_{ik}b_{kj}
$$

### 1.4 矩阵代数

#### 1.4.1 代数法则

1. $$A + B = B + A$$
2. $$(A + B) + C = A + (B + C)$$
3. $$(AB)C = A(BC)$$
4. $$A(B + C) = AB + AC$$
5. $$(A + B)C = AC + BC$$
6. $$(\alpha\beta)A = \alpha(\beta A)$$
7. $$\alpha(AB) = (\alpha A)B = A(\alpha B)$$
8. $$(\alpha + \beta)A = \alpha A + \beta A$$
9. $$\alpha(A + B) = \alpha A + \alpha B$$

#### 1.4.2 单位矩阵

*定义* $$n \times n$$的**单位矩阵(identity matrix)**为矩阵$$I = (\delta_{ij})$$，其中
$$
\delta_{ij} = 
  \begin{cases}
    1  & \quad 当 i = j \\
    0  & \quad 当 i \neq j \\
  \end{cases}
$$


#### 1.4.3 矩阵的逆

*定义* 若存在一个矩阵$$B$$使得$$AB = BA = I$$，则称$$n \times n$$矩阵$$A$$为**非奇异的(nonsingular)**或**可逆的(invertible)**. 矩阵$$B$$称为$$A$$的**乘法逆元(multiplicative inverse)**.


#### 1.4.4 转置

* $$(A^T)^T = A$$
* $$(\alpha A)^T = \alpha A^T$$
* $$(A + B)^T = A^T + B^T$$
* $$(AB)^T = B^TA^T$$


### 1.5 初等矩阵

#### 1.5.1 等价方程组

给定一$$m \times n$$线性方程组$$A\boldsymbol{x} = \boldsymbol{b}$$，如果在两端同乘一个非奇异的$$m \times n$$矩阵$$M$$，得到它的一个等价方程组
$$
MA\boldsymbol{x} = M\boldsymbol{b}
$$
我们可以将一系列的非奇异的矩阵$$E_1, \dotsc, E_k$$应用到方程组$$A\boldsymbol{x} = \boldsymbol{b}$$，的两端，从而得到一个较为简单的方程组
$$
U\boldsymbol{x} = \boldsymbol{c}
$$
其中$$U = E_k\dotsm E_1A$$，且$$\boldsymbol{c} = E_k \dotsm E_1\boldsymbol{b}$$.

#### 1.5.2 初等矩阵

**类型I**

**第I类初等矩阵交换矩阵$$I$$的两行得到**

> 例如
$$
E_1 = 
\begin{bmatrix}
       0 & 1 & 0 \\
       1 & 0 & 0 \\
       0 & 0 & 1
\end{bmatrix}

$$

**类型II**

**第II类初等矩阵由单位矩阵$$I$$的某一行乘以一个非零常数得到

> 例如
$$
E_2 = 
\begin{bmatrix}
       1 & 0 & 0 \\
       0 & 1 & 0 \\
       0 & 0 & 3
\end{bmatrix}

$$

**类型III**

**第III类初等矩阵由单位矩阵$$I$$的某一行的倍数加到另一行得到

> 例如
$$
E_3 = 
\begin{bmatrix}
       1 & 0 & 3 \\
       0 & 1 & 0 \\
       0 & 0 & 1
\end{bmatrix}

$$

*定理 1.5.2.1* **若$$E$$为一初等矩阵，则$$E$$是非奇异的，且$$E^{-1}$$为一与它同类型的初等矩阵.**

*定义* 若存在一个有限初等矩阵的序列$$E_1, E_2, \dotsc, E_k$$，使得
$$
B = E_kE_{k-1}\dotsm E_1A
$$则称$$A$$与$$B$$为**行等价的(row equivalent)**.



*定理 1.5.2.2* 令$$A$$为一$$n \times n$$矩阵，则下列命题是等价的
* $$A$$是非奇异的
* $$A\boldsymbol{x} = 0$$公有平凡解0
* $$A$$与$$I$$等价

*推论 1.5.2.3* **当且仅当$$A$$非奇异时，$$n$$个未知量$$n$$个方程的线性方程组$$A\boldsymbol{x} = \boldsymbol{b}$$有惟一解.**


#### 1.5.3 对角矩阵和三角形矩阵

一个$$n \times n$$矩阵$$A$$，当$$i \gt j$$时，$$a_{ij} = 0$$，则称为**上三角形的(upper triangular)**; 当$$i \lt j$$时，$$a_{ij} = 0$$，则称为**下三角形的(lower triangular)**; 统称为**三角形的(triangular)**；如果当$$ i \neq j$$时，$$a_{ij} = 0$$，则称为**对角的(diagonal)**.


#### 1.5.4 三角形分解

如果矩阵$$L$$为对角元素为1的下三角形矩阵，我们称$$L$$为**单位下三角形矩阵(unit lower triangular)**. 将矩阵$$A$$分解为一个单位下三角形矩阵和一个严格上三角形矩阵$$U$$的乘积的过程，通常称为**$$LU$$分解($$LU$$ factorization)**.


### 1.6 分块矩阵

#### 1.6.1 分块乘法

一般地，假设矩阵各个分块是恰当的，则分块乘法如下，设
$$
A = \begin{bmatrix}
       A_{11} & \dotsc & A_{1t} \\
       \vdots &        &        \\
       A_{s1} & \dotsc & A_{st}
\end{bmatrix}
\quad 及 \quad B = \begin{bmatrix}
       B_{11} & \dotsc & B_{qr} \\
       \vdots &        &        \\
       B_{t1} & \dotsc & B_{tr}
\end{bmatrix}

$$
则
$$
AB = \begin{bmatrix}
       C_{11} & \dotsc & C_{1r} \\
       \vdots &        &        \\
       C_{s1} & \dotsc & C_{sr}
\end{bmatrix}
$$

其中
$$
C_{ij} = \sum_{k = 1}^tA_{ik}B_{kj}
$$













