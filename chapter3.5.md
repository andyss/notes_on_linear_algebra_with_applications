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