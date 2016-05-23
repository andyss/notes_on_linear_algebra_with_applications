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




