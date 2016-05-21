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

令$$A$$为一$$m\times n$$矩阵，令$$N(A)$$为所有齐次方程组$$A\boldsymbol{x} = 0$$的解的集合. 于是
$$
N(A) = \{\boldsymbol{x} \in R^n  \mid  A\boldsymbol{x} = 0\}
$$子空间$$N(A)$$ 称为$$A$$的**零空间(nullspace)**.


#### 3.2.2 向量集合的张成

**定义** 令$$\boldsymbol{v_1, v_2, \dotsc, v_n}$$为向量空间$$V$$中的向量. $$\alpha_1\boldsymbol{v_1} + \alpha_2\boldsymbol{v_2} + \dotsb + \alpha_n\boldsymbol{v_n}(其中\alpha_1, \alpha_2, \dotsc, \alpha_n为标量)$$称为向量$$\boldsymbol{v_1, v_2, \dotsc, v_n}$$的**线性组合(linear combination)**. 向量$$\boldsymbol{v_1, v_2, \dotsc, v_n}$$的所有线性组合构成的集合称为$$\boldsymbol{v_1, v_2, \dotsc, v_n}$$的**张成(span)**. 向量$$\boldsymbol{v_1, v_2, \dotsc, v_n}$$的张成记为$$Span(\boldsymbol{v_1, v_2, \dotsc, v_n})$$.

**定理** 若$$\boldsymbol{v_1, v_2, \dotsc, v_n}$$为向量空间$$V$$中的元素，则$$Span(\boldsymbol{v_1, v_2, \dotsc, v_n})$$为$$V$$的一个子空间


#### 3.2.3 向量空间的张集

令$$\boldsymbol{v_1, v_2, \dotsc, v_n}$$为向量空间$$V$$中的向量. 我们用$$Span(\boldsymbol{v_1, v_2, \dotsc, v_n})$$表示由向量$$\boldsymbol{v_1, v_2, \dotsc, v_n}$$张成的$$V$$的子空间. 可能有$$Span(\boldsymbol{v_1, v_2, \dotsc, v_n}) = V$$的情形，此时，我们说向量$$\boldsymbol{v_1, v_2, \dotsc, v_n}$$张成$$V$$，或者$$\{\boldsymbol{v_1, v_2, \dotsc, v_n}\}$$是$$V$$的一个**张集(spanning set)**

**定义** $$\{\boldsymbol{v_1, v_2, \dotsc, v_n}\}$$是$$V$$的一个**张集(spanning set)**的充要条件为$$V$$中的每个向量都可以写成$$\{\boldsymbol{v_1, v_2, \dotsc, v_n}\}$$的一个线性组合.


### 3.3 线性无关

**定义** 如果向量空间$$V$$中的向量$$\boldsymbol{v_1, v_2, \dotsc, v_n}$$满足
$$
c_1\boldsymbol{v_1} + c_2\boldsymbol{v_2} + \dotsb + c_n\boldsymbol{v_n} = \boldsymbol{0}
$$就可以推出所有标量$$c_1, \dotsb, c_n$$必为0，则称它们为**线性无关的(linearly independent)**.

**定义** 如果存在不全为零的标量$$c_1, \dotsb, c_n$$, 使得向量空间$$V$$中的向量$$\boldsymbol{v_1, v_2, \dotsc, v_n}$$满足
$$
c_1\boldsymbol{v_1} + c_2\boldsymbol{v_2} + \dotsb + c_n\boldsymbol{v_n} = \boldsymbol{0}
$$则称它们为**线性相关的(linearly dependent)**.

**定理** 令$$\boldsymbol{x_1, x_2, \dotsc, x_n}$$为$$R^n$$中的$$n$$个向量，并令$$X = (x_1, x_2, \dotsc, x_n)$$. 向量$$\boldsymbol{x_1, x_2, \dotsc, x_n}$$线性相关的充要条件是$$X$$为奇异的.

**定理** 令$$\boldsymbol{v_1, v_2, \dotsc, v_n}$$为向量空间$$V$$中的向量，当且仅当$$\boldsymbol{v_1, v_2, \dotsc, v_n}$$线性无关时，$$Span(\boldsymbol{v_1, v_2, \dotsc, v_n})$$中的任一向量$$\boldsymbol{v}$$才可惟一地用向量$$\boldsymbol{v_1, v_2, \dotsc, v_n}$$的线性组合表示.


#### 3.3.1 函数的向量空间

**向量空间$$P_n$$**

为判断$$P_n$$中的多项式$$p_1, p_2, \dotsc, p_k$$是否线性无关，我们令
$$
c_1p_1 + c_2p_2 + \dotsb + c_kp_k = z
$$其中$$z$$表示零多项式
$$
z(x) = 0x^{n-1} + 0x^{n-2} + \dotsb + 0x + 0
$$若左则的多项式可写为$$a_1x^{n-1} + a_2x^{n-2} + \dotsb + a_{n-1}x + a_n$$的形式，则要使它线性无关，则$$a_i$$必全为0. 而且每一个$$a_i$$均为$$c_j$$的线性组合. 这个线性组合有平凡解，则多项式是线性无关的；否则，它们是线性相关的.

**向量空间$$C^{(n-1)}[a, b]$$**

**定义** 令$$f_1, f_2, \dotsc, f_n$$为$$C^{(n-1)}[a, b]$$的函数，定义$$[a, b]$$上的函数$$W[f_1, f_2, \dotsc, f_n](x)$$为
$$
W[f_1, f_2, \dotsc, f_n](x) = 
\left|\begin{array}{cccc}   
f_1(x) & f_2(x) & \dotsc & f_n(x) \\
f_1'(x) & f_2'(x) & \dotsc & f_n'(x) \\
\vdots & & & \\
f_1^{(n-1)}(x) & f_2^{(n-1)}(x) & \dotsc & f_n^{(n-1)}(x)
\end{array}\right|   
$$

函数$$W[f_1, f_2, \dotsc, f_n](x)$$称为$$f_1, f_2, \dotsc, f_n$$的**郎斯基行列式**.












