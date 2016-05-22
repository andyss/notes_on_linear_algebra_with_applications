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