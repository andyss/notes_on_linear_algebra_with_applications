### 3.1 定义

#### 3.1.1 欧几里得向量空间

也许最基本的向量空间就是欧几里得向量空间$$R^n$$，$$n = 1, 2, \dotsb$$.

一般的，$$R^n$$中的标量乘法和加法定义为
$$
\alpha\boldsymbol{x} = 
\begin{bmatrix}
\alpha x_1 \\
\alpha x_2 \\
\vdots \\
\alpha x_n
\end{bmatrix}
\quad 和 \quad \boldsymbol{x} + \boldsymbol{y} = 
\begin{bmatrix}
x_1 + y_1 \\
x_2 + y_2 \\
\vdots \\
x_n + y_n
\end{bmatrix}
$$

#### 3.1.2 向量空间$$R^{m\times n}$$

一般地，用$$R^{m\times n}$$表示所有$$m \times n$$实矩阵的集合. 若$$A = (a_{ij})$$，且$$B = (b_{ij})$$，则它们的和$$A + B$$定义为$$m\times n$$矩阵$$C = (c_{ij})$$，其中$$c_{ij} = a_{ij} + b_{ij}$$. 给定标量$$\alpha$$，可定义$$\alpha A$$为一$$m\times n$$矩阵，它的$$(i, j)$$元素为$$\alpha a_{ij}$$.

#### 3.1.3 向量空间的公理

**定义** 令$$V$$为一定义了加法和标题乘法运算的集合. 这意味着，对$$V$$中的每一对元素$$\boldsymbol{x}$$和$$\boldsymbol{y}$$，可惟一对就于$$V$$中的一个元素$$\boldsymbol{x} + \boldsymbol{y}$$，且对于每一个$$V$$中的元素$$\boldsymbol{x}$$和每一个标量$$\alpha$$，可以惟一对应于$$V$$中的元素$$\alpha\boldsymbol{x}$$. 如果集合$$V$$连同其上的加法和标量剩法运算满足下面的公理，则称为**向量空间(vector space)**.
1. 对$$V$$中的任何$$\boldsymbol{x}$$和$$\boldsymbol{y}$$，$$\boldsymbol{x} + \boldsymbol{y} = \boldsymbol{y} + \boldsymbol{x}$$
2. 对$$V$$中的任何$$\boldsymbol{x}$$，$$\boldsymbol{y}$$，$$\boldsymbol{z}$$，$$(\boldsymbol{x} + \boldsymbol{y}) + \boldsymbol{z} = \boldsymbol{x} + (\boldsymbol{y} + \boldsymbol{z})$$
3. $$V$$中存在一个元素$$\boldsymbol{0}$$，满足对任意的$$\boldsymbol{x} \in V$$有$$\boldsymbol{x} + \boldsymbol{0} = \boldsymbol{x}$$
4. 对每一个$$\boldsymbol{x} \in V$$，存在$$V$$中的一个元素$$-\boldsymbol{x}$$，满足$$\boldsymbol{x} + (-\boldsymbol{x}) = \boldsymbol{0}$$
5. 对任意的标量$$\alpha$$和$$V$$中的元素$$\boldsymbol{x}$$和$$\boldsymbol{y}$$，有$$\alpha(\boldsymbol{x} + \boldsymbol{y}) = \alpha\boldsymbol{x} + \alpha\boldsymbol{y}$$
6. 对任意标量$$\alpha$$和$$\beta$$及$$\boldsymbol{x} \in V$$，有$$(\alpha + \beta)\boldsymbol{x} = \alpha\boldsymbol{x} + \beta\boldsymbol{x}$$
7. 对任意标量$$\alpha$$和$$\beta$$及$$\boldsymbol{x} \in V$$，有$$(\alpha\beta)\boldsymbol{x} = \alpha(\beta\boldsymbol{x})$$
8. 对所有的$$\boldsymbol{x} \in V$$. 有$$1 \cdot \boldsymbol{x} = \boldsymbol{x}$$

#### 3.1.4 向量空间$$C[a, b]$$
