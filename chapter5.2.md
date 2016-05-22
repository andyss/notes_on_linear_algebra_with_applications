### 5.2 正交子空间

**定义** 设$$X$$和$$Y$$为$$R^n$$的子空间，若对每一$$\boldsymbol{x} \in X$$及$$\boldsymbol{y} \in Y$$都有$$\boldsymbol{x^Ty} = 0$$，则称$$X$$和$$Y$$为**正交的(orthogonal)**. 若$$X$$和$$Y$$是正交的，我们记为$$X\bot Y$$.

**定义** 令$$Y$$为$$R^n$$的子空间，$$R^n$$中所有与$$Y$$中的每一向量正交的向量集合记为$$Y^\bot$$. 因此
$$
Y^\bot = \{\boldsymbol{x} \in R^n\mid \boldsymbol{x}^T\boldsymbol{y} = 0，对每一个\boldsymbol{y} \in Y\}
$$集合$$Y^\bot$$称为$$Y$$的**正交补(orthogonal complement)**.

* 若$$X$$和$$Y$$为$$R^n$$中的正交子空间，则$$X \cap Y = \{\boldsymbol{0}\}$$
* 若$$Y$$为$$R^n$$的子空间，则$$Y^\bot$$也是$$R^n$$的子空间

#### 5.2.1 基本子空间

令$$A$$为一$$m\times n$$的矩阵，一个向量$$\boldsymbol{b} \in R^m$$在$$A$$的列空间中的充要条件是对某$$\boldsymbol{x} \in R^m$$，有$$\boldsymbol{b} = A\boldsymbol{x}$$. 如果将$$A$$看成是将$$R^n$$映射为$$R^m$$的线性变换，则$$A$$的列空间和$$A$$的值域是相同的，我们记$$A$$的值域为$$R(A)$$.则
$$
\begin{align*}
R(A) &= \{\boldsymbol{b}\in R^m \mid \boldsymbol{b} = A\boldsymbol{x}，对某\boldsymbol{x} \in R^n \} \\
&= A 的列空间
\end{align*}
$$
**定理** (基本子空间定理) 若$$A$$为一$$m\times n$$矩阵，则$$N(A) = R(A^T)^\bot$$, 且$$N(A^T) = R(A)^\bot$$.


**定理** 若$$S$$为$$R^n$$的一个子空间，则$$dimS + dimS^\bot = n$$. 此外，若$$\{x_1, \dotsc, x_r\}$$为$$S$$的一组基，且$$\{x_{r+1}, \dotsc, x_n\}$$为$$S^\bot$$的一组基，则$$\{x_1, \dotsc, x_n\}$$为$$R^n$$的一组基.

**定义** 若$$U$$和$$V$$为一个向量空间$$W$$的子空间，且每一个$$\boldsymbol{w} \in W$$可以惟一地写成一个和$$\boldsymbol{u + v}$$，其中$$\boldsymbol{u} \in U$$，且$$\boldsymbol{v} \in V$$，则我们称$$W$$为$$U$$与$$V$$的**直和(direct sum)**，并记为$$W = U\oplus V$$.

**定理** 若$$S$$为$$R^n$$的一个子空间，早
$$
R^n = S\oplus S^\bot
$$
