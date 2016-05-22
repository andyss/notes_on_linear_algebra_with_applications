

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
#### 2.3.3 向量长度

若$$\boldsymbol{x}$$是$$R^2$$或$$R^3$$中的一个向量，则$$\boldsymbol{x}$$的长度记为$$\|\boldsymbol{x}\|$$
$$
\|\boldsymbol{x}\| = (\boldsymbol{x}^T\boldsymbol{x})^{\frac{1}{2}}
$$











