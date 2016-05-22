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


