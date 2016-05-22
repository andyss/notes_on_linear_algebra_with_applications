### 4.2 线性变换的矩阵表示

**定理** 若$$L$$为一从$$R^n$$到$$R^m$$的线性变换，则存在一个$$m\times n$$矩阵$$A$$，使得对每一个$$\boldsymbol{x} \in R^n$$，有
$$
L(\boldsymbol{x}) = A\boldsymbol{x}
$$事实上，$$A$$的第$$j$$个列向量为
$$
\boldsymbol{a_j} = L(\boldsymbol{e_j})\quad j = 1, 2,\dotsc,n
$$
**定理** 若$$E = [\boldsymbol{v_1, v_2, \dotsc, v_n}]$$和$$F = [\boldsymbol{w_1, w_2, \dotsc, w_m}]$$分别为向量空间$$V$$和$$W$$的有序基，则对每一线性变换$$L: V \to W$$，存在一个$$m\times n$$矩阵$$A$$，使得对每一个$$\boldsymbol{v} \in V$$，有
$$
[L(\boldsymbol{v})]_F = A[\boldsymbol{v}]_E
$$$$A$$称为$$L$$收到应于有序基$$E$$和$$F$$的表示矩阵，事实上
$$
\boldsymbol{a_j} = [L(\boldsymbol{v_j})]_F，\quad j = 1, 2, \dotsc, n
$$
**定理** 令$$E = [\boldsymbol{u_1, \dotsc, u_n}]$$及$$F = [\boldsymbol{b_1, \dotsc, b_m}]$$分别为$$R^n$$和$$R^m$$的有序基. 若$$L: R^n \to R^m$$为一线性变换，且$$A$$为$$L$$相应于$$E$$和$$F$$的表示矩阵，则
$$
\boldsymbol{a_j} = B^{-1}L(\boldsymbol{u_j}), \quad j = 1, \dotsc, n
$$其中$$B = (\boldsymbol{b_1, \dotsc, b_m})$$.


**推论** 若$$A$$为线性变换$$L: R^n \to R^m$$相应于基
$$
E = [\boldsymbol{u_1, \dotsc, u_n}]\quad 和 \quad F = [\boldsymbol{b_1, \dotsc, b_m}]
$$的表示矩阵，则$$(\boldsymbol{b_1, \dotsc, b_m} \mid L(\boldsymbol{u_1}), \dotsc, L(\boldsymbol{u_n}))$$的行最简形为$$(I\mid A)$$.

#### 4.2.1 齐次坐标

**齐次坐标系(homogeneous coordinate system)**是通过将$$R^2$$中的向量等同于$$R^3$$中和该向量前两个坐标相同，而第三个坐标为1的向量来构造的.
$$
\begin{bmatrix}
x_1 \\
x_2
\end{bmatrix} \leftrightarrow 
\begin{bmatrix}
x_1 \\
x_2 \\
1
\end{bmatrix}
$$

> 例如
$$
\begin{bmatrix}
3 & 0 \\
0 & 3
\end{bmatrix} \to 
\begin{bmatrix}
3 & 0 & 0 \\
0 & 3 & 0 \\
0 & 0 & 1
\end{bmatrix}
$$
