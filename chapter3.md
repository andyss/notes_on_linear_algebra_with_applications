
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

**定理** 令$$f_1, f_2, \dotsc, f_n$$为$$C^{(n-1)}[a, b]$$的函数. 若在$$[a, b]$$中存在一个点$$x_0$$，使得$$W[f_1, f_2, \dotsc, f_n](x_0) \neq 0$$，则$$f_1, f_2, \dotsc, f_n$$线性无关.


### 3.4 基和维数

**定义** 当且仅当向量空间$$V$$中的向量$$\boldsymbol{v_1, v_2, \dotsc, v_n}$$满足
* $$\boldsymbol{v_1, v_2, \dotsc, v_n}$$线性无关
* $$\boldsymbol{v_1, v_2, \dotsc, v_n}$$张成$$V$$

时，称它们是微量空间$$V$$的**基(basis)**。

**定理** 若$$\{\boldsymbol{v_1, v_2, \dotsc, v_n}\}$$为向量空间$$V$$的一个张集，则$$V$$中的任何$$m$$个向量必线性相关，其中$$m \gt n$$.

**推论** 若$$\{\boldsymbol{v_1, v_2, \dotsc, v_n}\}$$和$$\{\boldsymbol{u_1, u_2, \dotsc, u_m}\}$$均为向量空间$$V$$的基，则$$n = m$$.

**定义** 令$$V$$为一向量空间，若$$V$$的一组基含有$$n$$个向量，我们称$$V$$的**维数(dimension)**为$$n$$. $$V$$的子空间$$\{\boldsymbol{0}\}$$的维数为0. 如果有有限多个向量张成$$V$$. 则称$$V$$是**有限维的(finite-dimensional)**. 否则，称$$V$$是**无限维的(infinite-dimensional)**.


**定理** 若$$V$$是维数$$n \gt 0$$的向量空间，则：
* 任意$$n$$个线性无关的向量张成$$V$$
* 任何张成$$V$$的$$n$$个向量是线性无关的

**定理** 若$$V$$是维数$$n \gt 0$$的向量空间，则：
* 没有少于$$n$$个的向量构成的集合可以张成$$V$$
* 任何少于$$n$$个线性无关的向量构成的子集可以扩展为$$V$$的一组基
* 任何多于$$n$$个向量的张集均可通过删除其中的向量得到$$V$$的一组基

#### 3.4.1 标准基

集合$$\{\boldsymbol{e_1, e_2, e_3}\}$$为$$R^3$$的**标准基(standard basis)**. 更一般的，$$R^n$$的标准基为集合$$\{\boldsymbol{e_1, e_2, \dotsc, e_n}\}$$.

例如$$R^{2\times 2}$$的标准基为$$\{E_{11}, E_{12}, E_{21}, E_{22}\}$$. $$E_{11} = [\begin{smallmatrix}
1&0 \\ 0&0
\end{smallmatrix}]$$，$$E_{12} = [\begin{smallmatrix}
0&1 \\ 0&0
\end{smallmatrix}]$$，$$E_{21} = [\begin{smallmatrix}
0&0 \\ 1&0
\end{smallmatrix}]$$，$$E_{22} = [\begin{smallmatrix}
0&0 \\ 0&1
\end{smallmatrix}]$$.

$$P_n$$的标准基为$$\{1, x, x^2, \dotsc, x^{n-1}\}$$


### 3.5 基变换

**定义** 令$$V$$为一向量空间，且令$$E = [\boldsymbol{v_1, v_2, \dotsc, v_n}]$$为$$V$$的一组有序基. 若$$\boldsymbol{v}$$为$$V$$中的一元素，则$$\boldsymbol{v}$$可写成为
$$
\boldsymbol{v} = c_1\boldsymbol{v_1} + c_2\boldsymbol{v_2} + \dotsb + c_n\boldsymbol{v_n}
$$其中$$c_1, c_2, \dotsc, c_n$$为标量. 因此可以将每一个向量$$\boldsymbol{v}$$惟一对应于$$R^n$$中的一个向量$$\boldsymbol{c} = (c_1, c_2, \dotsc, c_n)^T$$.  采用这种方式定义的向量$$\boldsymbol{c}$$称为$$\boldsymbol{v}$$相应于有序基$$E$$的**坐标向量(coordinate vector)**，并记为$$[\boldsymbol{v}]_E$$. $$c_i$$称为$$\boldsymbol{v}$$相对于$$E$$的**坐标(coordinate)**.

我们给定$$U = [\boldsymbol{u_1, u_2}]$$， 求对应于$$[\boldsymbol{e_1, e_2}]$$的坐标向量$$\boldsymbol{x}$$，我们只需要用$$U$$乘以$$\boldsymbol{c}$$:
$$
\boldsymbol{x} = U\boldsymbol{c}
$$矩阵$$U$$称为从有序基$$[\boldsymbol{u_1, u_2}]$$到基$$[\boldsymbol{e_1, e_2}]$$的**转移矩阵(transition matrix)**.

一般的，从$$[\boldsymbol{v_1, v_2, \dotsc, v_n}]$$到$$[\boldsymbol{u_1, u_2, \dotsc, u_n}]$$的转移矩阵
$$
S = U^{-1}V
$$
### 3.6 行空间和列空间

**定义** 如果$$A$$为一$$m\times n$$矩阵，由$$A$$的行向量张成的$$R^{1\times n}$$的子空间称为$$A$$的**行空间(row space)**. 由$$A$$的各列张成的$$R^m$$的子空间称为$$A$$的**列空间(column space)**.

**定理** 两个行等价的矩阵有相同的行空间.

**定义** $$A$$的行空间的维数称为矩阵$$A$$的**秩(rank)**

#### 3.6.1 线性方程组

**定理** 一个线性方程组$$A\boldsymbol{x} = \boldsymbol{b}$$相容的充要条件是$$\boldsymbol{b}$$在$$A$$的列空间中.

**定理** 令$$A$$为一$$m\times n$$矩阵. 当且仅当$$A$$的列向量张成$$R^m$$时，对每一$$\boldsymbol{b} \in R^m$$，线性方程组$$A\boldsymbol{x} = \boldsymbol{b}$$是相容的. 当且仅当$$A$$的列向量线性无关时，对每一$$\boldsymbol{b} \in R^m$$，方程组$$A\boldsymbol{x} = \boldsymbol{b}$$至多有一个解.

**推论** 当且仅当一个$$n\times n$$矩阵$$A$$的列向量为$$R^n$$的一组基时，$$A$$是非奇异的.

一般地，矩阵的秩和其零空间的维数加起来等于矩阵的列数. 一个矩阵的零空间的维数称为矩阵的**零度(nullity)**.

**定理** 若$$A$$为一$$m\times n$$矩阵，则$$A$$的秩与$$A$$的零度的和为$$n$$.


**定理** 若$$A$$为一$$m\times n$$矩阵，则$$A$$的行空间的维数等于$$A$$的列空间的维数.







