### 1.4 矩阵代数

#### 1.4.1 代数法则

1. $$A + B = B + A$$
2. $$(A + B) + C = A + (B + C)$$
3. $$(AB)C = A(BC)$$
4. $$A(B + C) = AB + AC$$
5. $$(A + B)C = AC + BC$$
6. $$(\alpha\beta)A = \alpha(\beta A)$$
7. $$\alpha(AB) = (\alpha A)B = A(\alpha B)$$
8. $$(\alpha + \beta)A = \alpha A + \beta A$$
9. $$\alpha(A + B) = \alpha A + \alpha B$$

#### 1.4.2 单位矩阵

**定义** $$n \times n$$的**单位矩阵(identity matrix)**为矩阵$$I = (\delta_{ij})$$，其中
$$
\delta_{ij} = 
  \begin{cases}
    1  & \quad 当 i = j \\
    0  & \quad 当 i \neq j \\
  \end{cases}
$$


#### 1.4.3 矩阵的逆

**定义** 若存在一个矩阵$$B$$使得$$AB = BA = I$$，则称$$n \times n$$矩阵$$A$$为**非奇异的(nonsingular)**或**可逆的(invertible)**. 矩阵$$B$$称为$$A$$的**乘法逆元(multiplicative inverse)**.


#### 1.4.4 转置

* $$(A^T)^T = A$$
* $$(\alpha A)^T = \alpha A^T$$
* $$(A + B)^T = A^T + B^T$$
* $$(AB)^T = B^TA^T$$

