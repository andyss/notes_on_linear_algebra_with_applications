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

*定义* 若存在一个矩阵$$B$$使得











