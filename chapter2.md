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
**定理** 

