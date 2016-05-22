### 3.2 子空间

**定义** 若$$S$$为向量空间$$V$$的非空子集，且$$S$$满足如下条件：
* 对任意标量$$\alpha$$，若$$\boldsymbol{x} \in S$$，则$$\alpha\boldsymbol{x} \in S$$
* 若$$\boldsymbol{x} \in S$$且$$\boldsymbol{y} \in S$$，则$$\boldsymbol{x} + \boldsymbol{y} \in S$$

则$$S$$称为$$V$$的**子空间(subspace)**.

**向量空间的任何子空间仍为向量空间.**


#### 3.2.1 矩阵的零空间

令$$A$$为一$$m\times n$$矩阵，令$$N(A)$$为所有齐次方程组$$A\boldsymbol{x} = 0$$的解的集合. 于是
$$
N(A) = \{\boldsymbol{x} \in R^n  \mid  A\boldsymbol{x} = 0\}
$$子空间$$N(A)$$ 称为$$A$$的**零空间(nullspace)**.


#### 3.2.2 向量集合的张成

**定义** 令$$\boldsymbol{v_1, v_2, \dotsc, v_n}$$为向量空间$$V$$中的向量. $$\alpha_1\boldsymbol{v_1} + \alpha_2\boldsymbol{v_2} + \dotsb + \alpha_n\boldsymbol{v_n}(其中\alpha_1, \alpha_2, \dotsc, \alpha_n为标量)$$称为向量$$\boldsymbol{v_1, v_2, \dotsc, v_n}$$的**线性组合(linear combination)**. 向量$$\boldsymbol{v_1, v_2, \dotsc, v_n}$$的所有线性组合构成的集合称为$$\boldsymbol{v_1, v_2, \dotsc, v_n}$$的**张成(span)**. 向量$$\boldsymbol{v_1, v_2, \dotsc, v_n}$$的张成记为$$Span(\boldsymbol{v_1, v_2, \dotsc, v_n})$$.

**定理** 若$$\boldsymbol{v_1, v_2, \dotsc, v_n}$$为向量空间$$V$$中的元素，则$$Span(\boldsymbol{v_1, v_2, \dotsc, v_n})$$为$$V$$的一个子空间


#### 3.2.3 向量空间的张集

令$$\boldsymbol{v_1, v_2, \dotsc, v_n}$$为向量空间$$V$$中的向量. 我们用$$Span(\boldsymbol{v_1, v_2, \dotsc, v_n})$$表示由向量$$\boldsymbol{v_1, v_2, \dotsc, v_n}$$张成的$$V$$的子空间. 可能有$$Span(\boldsymbol{v_1, v_2, \dotsc, v_n}) = V$$的情形，此时，我们说向量$$\boldsymbol{v_1, v_2, \dotsc, v_n}$$张成$$V$$，或者$$\{\boldsymbol{v_1, v_2, \dotsc, v_n}\}$$是$$V$$的一个**张集(spanning set)**

**定义** $$\{\boldsymbol{v_1, v_2, \dotsc, v_n}\}$$是$$V$$的一个**张集(spanning set)**的充要条件为$$V$$中的每个向量都可以写成$$\{\boldsymbol{v_1, v_2, \dotsc, v_n}\}$$的一个线性组合.

