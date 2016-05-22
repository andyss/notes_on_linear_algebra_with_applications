### 5.1 $$R^n$$中的标量积

**定义** 乘积$$\boldsymbol{x}^T\boldsymbol{y}$$称为$$\boldsymbol{x}$$和$$\boldsymbol{y}$$的**标量积(scalar product)**

#### 5.1.1 $$R^n$$中的正交性

**定理** 若$$\boldsymbol{x}$$和$$\boldsymbol{y}$$为$$R^2$$或$$R^3$$中的两个非零向量，且$$\theta$$为它们的夹角，则
$$
\boldsymbol{x}^T\boldsymbol{y} = \|\boldsymbol{x}\| \|\boldsymbol{y}\| cos\theta
$$
**推论** (柯西-施瓦茨不等式) 若$$\boldsymbol{x}$$和$$\boldsymbol{y}$$为$$R^2$$或$$R^3$$中的向量，则
$$
|\boldsymbol{x}^T\boldsymbol{y}| \leq \|\boldsymbol{x}\| \|\boldsymbol{y}\|
$$当且仅当其中一个向量为$$\boldsymbol{0}$$，或一个向量为另一个向量的倍数时，等号成立.

若$$\boldsymbol{x}^T\boldsymbol{y} = 0$$，则$$R^2（或者R^3)$$中的向量$$\boldsymbol{x}$$和$$\boldsymbol{y}$$称为**正交的(orthogonal)**.

**定义** 标量$$\alpha$$满足
$$
\alpha = \|\boldsymbol{x}\| cos\theta = \frac{\|\boldsymbol{x}\| \|\boldsymbol{y}\| cos\theta}{\|\boldsymbol{y}\|} = \frac{\boldsymbol{x}^T\boldsymbol{y}}{\|\boldsymbol{y}\|}
$$标量$$\alpha$$称为$$\boldsymbol{x}$$到$$\boldsymbol{y}$$的**标量投影(scalar projection)**，且向量$$\boldsymbol{p}$$称为$$\boldsymbol{x}$$到$$\boldsymbol{y}$$的**向量投影(vector projection)**，其中$$\boldsymbol{p} = \alpha \boldsymbol{u}$$，$$\boldsymbol{u}$$为$$\boldsymbol{y}$$方向上的单位向量(长度为1).


$$\boldsymbol{x}$$到$$\boldsymbol{y}$$的标量投影：
$$
\alpha = \frac{\boldsymbol{x}^T\boldsymbol{y}}{\|\boldsymbol{y}\|}
$$
$$\boldsymbol{x}$$到$$\boldsymbol{y}$$的向量投影：
$$
\boldsymbol{p} = \alpha\boldsymbol{u} = \alpha\frac{1}{\|\boldsymbol{y}\|}\boldsymbol{y} = \frac{\boldsymbol{x}^T\boldsymbol{y}}{\boldsymbol{y}^T\boldsymbol{y}}\boldsymbol{y}
$$


若$$\boldsymbol{x} \in R^n$$，则$$\boldsymbol{x}$$的**欧几里得长度**定义为
$$
\|\boldsymbol{x}\| = (\boldsymbol{x}^T\boldsymbol{x})^{1/2} 
$$若$$\boldsymbol{x}$$和$$\boldsymbol{y}$$为$$R^n$$中的两个向量，则向量之间的距离为$$\|\boldsymbol{y} - \boldsymbol{x}\|$$. 对$$R^n$$中的任何非零向量$$\boldsymbol{x}$$和$$\boldsymbol{y}$$，有
$$
-1 \leq \frac{\boldsymbol{x}^T\boldsymbol{y}}{\|\boldsymbol{x}\| \|\boldsymbol{y}\|} \leq 1
$$因此两个$$R^n$$中的向量$$\boldsymbol{x}$$和$$\boldsymbol{y}$$的夹角$$\theta$$定义为
$$
cos\theta = \frac{\boldsymbol{x}^T\boldsymbol{y}}{\|\boldsymbol{x}\| \|\boldsymbol{y}\|}, \quad 0 \leq \theta \leq \pi
$$
通常，为了方便，使用单位向量比较简便，如果令
$$
\boldsymbol{u} = \frac{1}{\|\boldsymbol{x}\|}\boldsymbol{x} \quad 且 \quad \boldsymbol{v} = \frac{1}{\|\boldsymbol{y}\|}\boldsymbol{y}
$$
则
$$
cos\theta = \boldsymbol{u}^T\boldsymbol{v}
$$
若$$\boldsymbol{x}^T\boldsymbol{y} = 0$$，则向量$$\boldsymbol{x}$$和$$\boldsymbol{y}$$称为**正交的(orthogonal)**. 记为$$\boldsymbol{x}\bot\boldsymbol{y}$$.

若$$\boldsymbol{x}$$和$$\boldsymbol{y}$$为$$R^n$$中的向量，早
$$
\|\boldsymbol{x} + \boldsymbol{y}\| = (\boldsymbol{x} + \boldsymbol{y})^T(\boldsymbol{x} + \boldsymbol{y}) = \|\boldsymbol{x}\|^2 + 2\boldsymbol{x}^T\boldsymbol{y} + \|\boldsymbol{y}\|^2
$$当$$\boldsymbol{x}$$和$$\boldsymbol{y}$$正交时，方程称为**毕达哥拉斯定律(Pythagorean Law)**.
$$
\|\boldsymbol{x} + \boldsymbol{y}\|^2 = \|\boldsymbol{x}\|^2 + \|\boldsymbol{y}\|^2 
$$