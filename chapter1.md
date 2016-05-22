



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

**定理 1.5.2.1** **若$$E$$为一初等矩阵，则$$E$$是非奇异的，且$$E^{-1}$$为一与它同类型的初等矩阵.**

**定义** 若存在一个有限初等矩阵的序列$$E_1, E_2, \dotsc, E_k$$，使得
$$
B = E_kE_{k-1}\dotsm E_1A
$$则称$$A$$与$$B$$为**行等价的(row equivalent)**.



**定理 1.5.2.2** 令$$A$$为一$$n \times n$$矩阵，则下列命题是等价的
* $$A$$是非奇异的
* $$A\boldsymbol{x} = 0$$公有平凡解0
* $$A$$与$$I$$等价

**推论 1.5.2.3** 当且仅当$$A$$非奇异时，$$n$$个未知量$$n$$个方程的线性方程组$$A\boldsymbol{x} = \boldsymbol{b}$$有惟一解.


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
#### 1.6.2 外积展开

我们称
$$
\boldsymbol{x}^T\boldsymbol{y} = (x_1, x_2, \dotsc, x_n)
\begin{bmatrix}
       y_1 \\
       y_2 \\
       \vdots \\
       y_n
\end{bmatrix}
= x_1y_1 + x_2y_2 + \dotsb + x_ny_n
$$
这种乘积称为**标量积(scalar product)**或**内积(inner product)**.


我们将
$$
\boldsymbol{xy}^T = \begin{bmatrix}
       x_1 \\
       x_2 \\
       \vdots \\
       x_n
\end{bmatrix}
(y_1, y_2, \dotsc, y_n) = 
\begin{bmatrix}
       x_1y_1 & x_2y_2 & \dotsc & x_1y_n \\
       x_2y_1 & x_2y_2 & \dotsc & x_2y_n \\
       \vdots &        &        &        \\
       x_ny_1 & x_ny_2 & \dotsc & x_ny_n
\end{bmatrix}
$$

这种乘积称为**外积(outer product)**.


我们可以推广到矩阵，
$$
XY^T = \boldsymbol{(x_1, x_2, \dotsc, x_n)}
\begin{bmatrix}
\boldsymbol{
       y_1^T \\
       y_2^T \\
       \vdots \\
       y_n^T
}
\end{bmatrix}
= \boldsymbol{x_1y_1^T + x_2y_2^T + \dotsb + x_ny_n^T} 

$$
称为**外积展开(outer product expansion)**.















