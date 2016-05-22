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

