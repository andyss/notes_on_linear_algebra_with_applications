### 5.4 内积空间

**定义** 一个微量空间$$V$$上的**内积(inner product)**为$$V$$上的运算，它将$$V$$中的向量$$\boldsymbol{x}$$和$$\boldsymbol{y}$$与一个实数$$\langle\boldsymbol{x}, \boldsymbol{y}\rangle$$关联，并满足下列条件
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

