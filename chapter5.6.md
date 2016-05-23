### 5.6 格拉姆-施密特正交化过程

**定理** (格拉姆-施密特过程) 令$$\{\boldsymbol{x_1, x_2, \dotsc, x_n}\}$$为一内积空间$$V$$的一组基，令
$$
\boldsymbol{u_1} = \left(\frac{1}{\|\boldsymbol{x_1}\|}\right) \boldsymbol{x_1}
$$并递归的定义$$\boldsymbol{u_2, \dotsc, u_n}$$为
$$
\boldsymbol{u_{k+1}} = \frac{1}{\|\boldsymbol{x_{k+1} - p_k} \|}(\boldsymbol{x_{k+1}} - \boldsymbol{p_k}), \quad k = 1, \dotsc, n - 1
$$其中
$$
\boldsymbol{p_k} = \langle \boldsymbol{x_{k+1}}, \boldsymbol{u_1}\rangle\boldsymbol{u_1} + \langle\boldsymbol{x_{k+1}}, \boldsymbol{u_2}\rangle\boldsymbol{u_2} + \dotsb + \langle\boldsymbol{x_{k+1}}, \boldsymbol{u_k}\rangle\boldsymbol{u_k}
$$为$$\boldsymbol{x_{k+1}}$$到$$Span(\boldsymbol{u_1, u_2, \dotsc, u_n})$$上的投影向量，集合
$$
\{\boldsymbol{u_1, u_2, \dotsc, u_n}\}
$$即为$$V$$的一组规范正交基




