### 2.1 矩阵的行列式

**定义** 令$$A=(a_{ij})$$为一$$n\times n$$矩阵，并用$$M_{ij}$$表示删除$$A$$中包含$$a_{ij}$$的行和列得到的$$(n-1)\times (n-1)$$矩阵，矩阵$$M_{ij}$$的行列式称为$$a_{ij}$$的**子式(minor)**. 定义$$a_{ij}$$的**余子式(cofactor)**$$A_{ij}$$为
$$
A_{ij} = (-1)^{i+j}det(M_{ij})
$$
例如$$det(A) = a_{11}A_{11} + a_{12}A_{12}$$，则称为$$det(A)$$按$$A$$的第一行的**余子式展开(confactor expansion)**.


**定义** 一个$$n\times n$$矩阵$$A$$的**行列式(determinant)**，记为$$det(A)$$，是一个与矩阵$$A$$对应的标量，它可如下递归定义
$$
det(A) =   
\begin{cases}
    a_{11}  & \quad 当 n = 1 时 \\
    a_{11}A_{11} + a_{12}A_{12} + \dotsb + a_{1n}A_{1n}  & \quad 当 n \gt 1 时 \\
\end{cases}

$$
其中
$$
A_{ij} = (-1)^{1+j}det(M_{1j}), j = 1, \dotsc, n
$$
**定理** 设$$A$$为一$$n \times n$$矩阵，其中$$n \geq 2$$，则$$det(A)$$可表示为$$A$$的任何行或列的余子式展开，即
$$
\begin{align}
det(A) = a_{i1}A_{i1} + a_{i2}A_{i2} + \dotsb + a_{in}A_{in} \\
=  a_{1j}A_{1j} + a_{2j}A_{2j} + \dotsb + a_{nj}A_{nj} \\
\end{align}
$$
其中$$i=1, \dotsc, n, 且j = 1, \dotsc, n$$.

**定理** 设$$A$$为一$$n\times n$$矩阵，则$$det(A^T) = det(A)$$.

**定理** 设$$A$$为一$$n\times n$$三角形矩阵，则$$A$$的行列式等于$$A$$的对角元素的乘积.

**定理** 设$$A$$为一$$n\times n$$矩阵
* 若$$A$$有一行或一列包含的元素全为零，则$$det(A) = 0 $$
* 若$$A$$有两行或者两列相等，则$$det(A) = 0$$

### 2.2 行列式的性质

**引理** 令$$A$$为一$$n\times n$$矩阵，若$$A_{jk}$$表示$$a_{jk}$$的余子式，其中$$k = 1, \dotsc, n$$，则
$$
a_{i1}A_{j1} + a_{i2}A_{j2} + \dotsb + a_{in}A_{jn} = 
\begin{cases}
    det(A)  & \quad 当 i = j 时 \\
    0  & \quad 当 n \neq j 时 \\
\end{cases}
$$

** 行运算I ** 交换$$A$$的两行

$$
det(E_1A) = -det(A)
$$

> 例如
$$
E_1 = \begin{bmatrix}
0 & 1 \\
1 & 0 
\end{bmatrix}
$$

** 行运算II ** $$A$$的某一行乘以一个非零常数
$$
det(E_2A) = det(E_2)det(A)
$$
** 行运算III ** 某一行的倍数加到其他行
$$
det(E_3A) = det(A) = det(E_3)det(A)
$$

**总结**

若$$E$$为一初等矩阵，则
$$
det(EA) = det(E)det(A)
$$
其中
$$
det(E) = 
\begin{cases}
    -1  & \quad 当 E 为第I类初等矩阵 \\
    \alpha \neq 0  & \quad 当 E 为第II类初等矩阵 时 \\
    1  & \quad 当 E 为第III类初等矩阵 时 \\
\end{cases}

$$

**定理** 一个$$n \times n$$矩阵$$A$$是奇异的充要条件为
$$
det(A) = 0
$$
**定理** 若$$A$$和$$B$$均为$$n\times n$$矩阵，则
$$
det(AB) = det(A)det(B)
$$
### 2.3 其它

#### 2.3.1 伴随矩阵

我们定义
$$
adj A = 
\begin{bmatrix}
A_{11} & A_{21} & \dotsc & A_{n1} \\
A_{12} & A_{22} & \dotsc & A_{n2} \\
\vdots &        &        &        \\
A_{1n} & A_{2n} & \dotsc & A_{nn} 
\end{bmatrix}
$$
为矩阵$$A$$的**伴随(adjoint)**. 其中原矩阵元素用它们的余子式替换.


**求逆**

若$$A$$为非奇异的，则$$det(A) \neq 0 $$，因此
$$
A^{-1} = \frac{1}{det(A)}adj A, 其中det(A) \neq 0
$$

#### 2.3.2 克拉默法则

** 定理 ** 令$$A$$为一$$n\times n$$非奇异矩阵，并令$$\boldsymbol{b} \in R^n$$. 令$$A_i$$为将矩阵$$A$$中的第$$i$$列用$$\boldsymbol{b}$$替换得到的矩阵，若$$\boldsymbol{x}$$为方程组$$A\boldsymbol{x} = \boldsymbol{b}$$的惟一解，则
$$
x_i = \frac{det(A_i)}{det(A)}, \quad i = 1, 2, \dotsc, n
$$
#### 2.3.3 向量积










