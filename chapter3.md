



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







