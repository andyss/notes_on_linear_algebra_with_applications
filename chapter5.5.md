### 5.5 正交集

**定义** 令$$\boldsymbol{v_1, v_2, \dotsc, v_n}$$为一内积空间$$V$$中的非零向量，若当$$i \neq j$$时有$$\langle\boldsymbol{v_i}, \boldsymbol{v_j}\rangle = 0$$，则$$\{\boldsymbol{v_1, v_2, \dotsc, v_n}\}$$称为向量的**正交集(orthogonal set)**

**定理** 若$$\{\boldsymbol{v_1, v_2, \dotsc, v_n}\}$$为一内积空间$$V$$中的非零向量的正交集，则$$\boldsymbol{v_1, v_2, \dotsc, v_n}$$是线性无关的

**定义** **规范正交的(orthonormal)**向量集合是单位向量的正交集

集合$$\{\boldsymbol{u_1, u_2, \dotsc, u_n}\}$$是规范正交集的充要条件为
$$
\langle\boldsymbol{u_i}, \boldsymbol{u_j}\rangle = \delta_{ij}
$$
其中
$$
\delta_{ij} = 
\begin{cases}
1, &\quad i = j \\
0, &\quad i \neq j
\end{cases}
$$

给定任意的正交非零向量集合$$\{\boldsymbol{v_1, v_2, \dotsc, v_n}\}$$，可以通过定义
$$
\boldsymbol{u_i} = \left(\frac{1}{\|\boldsymbol{v_i}\|}\right) \boldsymbol{v_i}, \quad i = 1, 2, \dotsc, n
$$构造一个规范正交集.


**定理** 令$$\{\boldsymbol{u_1, u_2, \dotsc, u_n}\}$$为一个内积空间$$V$$的规范正交基，若$$\boldsymbol{v} = \sum_{i = 1}^nc_i\boldsymbol{u_i}$$，则$$c_i = \langle\boldsymbol{v}, \boldsymbol{u_i}\rangle$$.

**推论** 令$$\{\boldsymbol{u_1, u_2, \dotsc, u_n}\}$$为一个内积空间$$V$$的规范正交基，若$$\boldsymbol{u} = \sum_{i = 1}^na_i\boldsymbol{u_i}$$及$$\boldsymbol{v} = \sum_{i = 1}^nb_i\boldsymbol{u_i}$$则
$$
\langle\boldsymbol{u}, \boldsymbol{v}\rangle = \sum_{i = 1}^n a_i b_i
$$
**推论** (帕塞瓦尔公式) 若$$\{\boldsymbol{u_1, u_2, \dotsc, u_n}\}$$为一个内积空间$$V$$的规范正交基，且$$\boldsymbol{v} = \sum_{i = 1}^nc_i\boldsymbol{u_i}$$，则
$$
\|\boldsymbol{v}\|^2 = \sum_{i = 1}^nc_i^2
$$

#### 5.5.1 正交矩阵

**定义** 若一个$$n\times n$$矩阵$$Q$$的列向量构成$$R^n$$中的一组规范正交基，则称$$Q$$为**正交矩阵(orthogonal matrix)**

**定理** 一个$$n\times n$$矩阵$$Q$$是正交矩阵的充要条件为$$Q^TQ = I$$

**正交矩阵的性质** 若$$Q$$为一$$n\times n$$正交矩阵，则
* $$Q$$的列向量构成了$$R^n$$的一组规范正交基
* $$Q^TQ = I$$
* $$Q^T = Q^{-1}$$
* $$\langle Q\boldsymbol{x}, Q\boldsymbol{y} \rangle = \langle\boldsymbol{x},\boldsymbol{y}\rangle$$
* $$\|Q\boldsymbol{x}\|_2 = \|\boldsymbol{x}\|_2$$

#### 5.5.2 置换矩阵

**置换矩阵(permutation matrix)**是将单位矩阵的各列重排得到的矩阵，显然置换矩阵为正交矩阵.


#### 5.5.3 规范正交集与最小二乘问题

**定理** 若$$A$$的列向量构成了$$R^n$$中的规范正交集，则$$A^TA = I$$且最小二乘问题的解为
$$
\widehat{\boldsymbol{x}} = A^T\boldsymbol{b}
$$

**定理** 令$$S$$为一个内积空间$$V$$的子空间，并令$$\boldsymbol{x} \in V$$，令$$\{\boldsymbol{u_1, u_2, \dotsc, u_n}\}$$为$$S$$的一组规范正交基，若
$$
p = \sum_{i = 1}^nc_i\boldsymbol{u_i}
$$其中对每一个$$i$$，
$$
c_i = \langle \boldsymbol{x}, \boldsymbol{u_i} \rangle
$$则$$\boldsymbol{p} - \boldsymbol{x} \in S^\bot$$

**定理** 在如上一定理的假设下，$$\boldsymbol{p}$$为$$S$$中最接近$$\boldsymbol{x}$$的元素，也就是说，对$$S$$中的任何$$\boldsymbol{y} \neq p$$，都有
$$
\|\boldsymbol{y} - \boldsymbol{x}\| \gt \|\boldsymbol{p} - \boldsymbol{x}\|
$$

**推论** 令$$S$$为$$R^m$$的一个非零子空间，并令$$\boldsymbol{b} \in R^m$$，若$$\{\boldsymbol{u_1, u_2, \dotsc, u_n}\}$$为$$S$$的一组规范正交基，且$$U = (\boldsymbol{u_1, u_2, \dotsc, u_n})$$，则$$\boldsymbol{b}$$到$$S$$上的投影$$\boldsymbol{p}$$为
$$
\boldsymbol{p} = UU^T\boldsymbol{b}
$$

#### 5.5.4 用三解多项式逼近

三解多项式用于逼近周期函数，所谓**$$n$$次三角多项式(trigonometric polynomial)**，是一个形如
$$
t_n(x) = \frac{a_0}{2} + \sum_{k = 1}^n(a_k\,\cos{kx} + b_k\,\sin{kx})
$$的函数

如果
$$
a_0 = \langle f, 1 \rangle = \frac{1}{\pi}\int_{-\pi}^{\pi}\,f(x)\mathrm{d}x
$$
且
$$
a_k = \langle f, \cos{kx}\rangle = \frac{1}{\pi}\int_{-\pi}^{\pi}\,f(x)\cos{kx}\mathrm{d}x \\

b_k = \langle f, \sin{kx}\rangle = \frac{1}{\pi}\int_{-\pi}^{\pi}\,f(x)\sin{kx}\mathrm{d}x \\

$$其中$$k = 1, 2, \dotsc, n$$，则这些系数确定了$$f$$的最优最小二乘逼近. $$a_k$$和$$b_k$$就是人们熟知的**傅里叶系统(Fourier coefficients)**.






