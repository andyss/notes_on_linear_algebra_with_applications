### 5.4 内积空间

**定义** 一个向量空间$$V$$上的**内积(inner product)**为$$V$$上的运算，它将$$V$$中的向量$$\boldsymbol{x}$$和$$\boldsymbol{y}$$与一个实数$$\langle\boldsymbol{x}, \boldsymbol{y}\rangle$$关联，并满足下列条件
1. $$\langle\boldsymbol{x}, \boldsymbol{y}\rangle \geq 0$$，等号成立的充要条件是$$\boldsymbol{x} = 0$$
2. 对$$V$$中所有的$$\boldsymbol{x}$$和$$\boldsymbol{y}$$，有$$\langle\boldsymbol{x}, \boldsymbol{y}\rangle = \langle\boldsymbol{y}, \boldsymbol{x}\rangle$$
3. 对$$V$$中所有的$$\boldsymbol{x},\boldsymbol{y}, \boldsymbol{z}$$，及所有标量$$\alpha$$和$$\beta$$，有$$\langle\alpha\boldsymbol{x} + \beta\boldsymbol{y}, \boldsymbol{z}\rangle = \alpha\langle\boldsymbol{x}, \boldsymbol{z}\rangle + \beta\langle\boldsymbol{y}, \boldsymbol{z}\rangle$$

#### 5.4.1 向量空间$$R^n$$

$$R^n$$中的标准内积就是标量积
$$
\langle\boldsymbol{x}, \boldsymbol{y}\rangle = \boldsymbol{x}^T\boldsymbol{y}
$$
给定一个元素为正的向量$$\boldsymbol{w}$$，我们也可以定义$$R^n$$上的一个内积为
$$
\langle\boldsymbol{x}, \boldsymbol{y}\rangle = \sum_{i = 1}^nx_iy_iw_i
$$
元素$$w_i$$称为**权(weights)**.

#### 5.4.2 向量空间$$R^{m\times n}$$

给定$$R^{m\times n}$$中的$$A$$和$$B$$，我们可以定义一个内积为
$$
\langle A, B\rangle = \sum_{i = 1}^m\sum_{j = 1}^na_{ij}b_{ij}
$$
#### 5.4.3 向量空间$$C[a, b]$$

在$$C[a, b]$$中，我们可以定义内积为
$$
\langle f, g\rangle = \int_a^bf(x)g(x)\mathrm{d}x
$$
注意到
$$
\langle f, f\rangle = \int_a^b(f(x))^2\mathrm{d}x \geq 0
$$
若$$w(x)$$为$$[a, b]$$上的一个正的连续函数，则
$$
\langle f, g\rangle = \int_a^bf(x)g(x)w(x)\mathrm{d}x
$$
也定义了一个$$C[a, b]$$上的内积，函数$$w(x)$$称为**权函数(weight function)**

#### 向量空间$$P_n$$

令$$x_1, x_2, \dotsc, x_n$$为不同的实数，对每一对$$P_n$$中的多项式，定义
$$
\langle p, q\rangle = \sum_{i = 1}^np(x_i)q(x_i)
$$
注意到
$$
\langle p, p\rangle = \sum_{i = 1}^n(p(x_i))^2 \geq 0
$$若$$w(x)$$为一正函数，则
$$
\langle p, q\rangle = \sum_{i = 1}^np(x_i)q(x_i)w(x_i)
$$
也定义了$$P_n$$上的一个内积


#### 内积空间的基本性质

若$$\boldsymbol{v}$$为内积空间$$V$$中的一个向量，则$$\boldsymbol{v}$$的**长度(length)**或**范数(norm)**定义为
$$
\|\boldsymbol{v}\| = \sqrt{\langle \boldsymbol{v}, \boldsymbol{v} \rangle}
$$
如果两个向量$$\boldsymbol{u}$$和$$\boldsymbol{v}$$满足$$\langle \boldsymbol{u}, \boldsymbol{v}\rangle = 0$$则称它们为**正交的(orthogonal)**

**定理** (毕达哥拉斯定理) 若$$\boldsymbol{u}$$和$$\boldsymbol{v}$$为一个内积空间$$V$$中的正交向量，则
$$
\|\boldsymbol{u} + \boldsymbol{v}\|^2 = \|\boldsymbol{u}\|^2 + \|\boldsymbol{v}\|^2
$$

**定义** 若$$\boldsymbol{u}$$和$$\boldsymbol{v}$$为内积空间$$V$$中的向量，且$$\boldsymbol{v} \neq \boldsymbol{0}$$，则$$\boldsymbol{u}$$到$$\boldsymbol{v}$$的**标量投影(scalar projection)**为
$$
\alpha = \frac{\langle\boldsymbol{u}, \boldsymbol{v}\rangle}{\|\boldsymbol{v}\|}
$$
且$$\boldsymbol{u}$$到$$\boldsymbol{v}$$的**向量投影(vector projection)**为
$$
\boldsymbol{p} = \alpha\left(\frac{1}{\|\boldsymbol{v}\|}\boldsymbol{v}\right) = \frac{\langle\boldsymbol{u}, \boldsymbol{v}\rangle}{\langle\boldsymbol{v}, \boldsymbol{v}\rangle}\boldsymbol{v}
$$

**定理** (柯西-施瓦茨不等式) 若$$\boldsymbol{u}$$和$$\boldsymbol{v}$$为内积空间$$V$$中的两个向量，则
$$
|\,\langle\boldsymbol{u}, \boldsymbol{u}\rangle\,| \leq \|\boldsymbol{u}\|\;\|\boldsymbol{v}\|
$$
#### 范数

**定义** 设$$V$$为一个向量空间，若对每一向量$$\boldsymbol{v} \in V$$，存在一个与之相关联的实数$$\|\boldsymbol{v}\|$$，称为$$\boldsymbol{v}$$的**范数(norm)**，它满足
1. $$\|\boldsymbol{v}\| \geq 0$$，其中等式成立的充要条件为$$\boldsymbol{v} = \boldsymbol{0}$$
2. 对任一标量$$\alpha$$，$$\|\alpha\boldsymbol{v}\| = |\alpha|\;\|\boldsymbol{v}\|$$
3. 对所有的$$\boldsymbol{v}, \boldsymbol{w} \in V, \|\boldsymbol{v} + \boldsymbol{w}\| \leq \|\boldsymbol{v}\| + \|\boldsymbol{w}\|$$
则称$$V$$为**线性赋范空间(normed linear space)**. 第三个条件称为**三角不等式(triangle inequality)**




