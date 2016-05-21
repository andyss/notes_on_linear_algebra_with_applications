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

用$$C[a, b]$$表示所有定义在闭区间$$[a, b]$$上的实值连续函数. 此时，全集为一函数集合. 我们定义$$C[a, b]$$中两个函数的和$$f + g$$定义为对所有$$[a, b]$$中的$$x$$,
$$
(f + g)(x) = f(x) + g(x)
$$新函数$$f + g$$也是$$C[a, b]$$的元素，因为两个连续函数的和仍为连续函数. 若$$f$$为$$C[a, b]$$中的函数, $$\alpha$$为一个实数，则$$\alpha f$$定义为对所有$$[a, b]$$中的$$x$$,
$$
(\alpha f)(x) = \alpha f(x)
$$而我们定义函数
$$
z(x) = 0, \quad 对所有[a, b]中的x
$$
为零向量.


#### 3.1.5 向量空间$$P_n$$

令$$P_n$$表示次数小于$$n$$的所有多项式的集合. 定义$$p + q$$和$$\alpha p$$为对所有的实数$$x$$，有
$$
(p + q)(x) = p(x) + q(x)
$$和
$$
(\alpha p)(x) = \alpha p(x)
$$
此时零向量是零多项式，
$$
z(x) = 0x^{n-1} + 0x^{n-2} + \dotsb + 0x + 0
$$
#### 3.1.6 向量空间的其他性质

**定理** 若$$V$$为向量空间，且$$x$$为$$V$$的任一元素，则
* $$0\boldsymbol{x} = \boldsymbol{0}$$
* $$\boldsymbol{x} + \boldsymbol{y} = 0$$蕴涵$$\boldsymbol{y} = -\boldsymbol{x}$$(即$$\boldsymbol{x}$$的加法逆元是惟一的)
* $$(-1)\boldsymbol{x} = -\boldsymbol{x}$$

### 3.2 子空间

**定义** 若$$S$$为向量空间$$V$$的非空子集，且$$S$$满足如下条件：
* 对任意标量$$\alpha$$，若$$\boldsymbol{x} \in S$$，则$$\alpha\boldsymbol{x} \in S$$
* 若$$\boldsymbol{x} \in S$$且$$\boldsymbol{y} \in S$$，则$$\boldsymbol{x} + \boldsymbol{y} \in S$$

则$$S$$称为$$V$$的**子空间(subspace)**.

**向量空间的任何子空间仍为向量空间.**


#### 3.2.1 矩阵的零空间



#### 3.2.2 向量集合的张成






