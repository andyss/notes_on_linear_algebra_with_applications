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

