### 4.1 定义

**定义** 一个将向量空间$$V$$映射到向量空间$$W$$的映射$$L$$，如果对所有$$\boldsymbol{v_1, v_2} \in V$$及所有的标量$$\alpha$$和$$\beta$$，
$$
L(\alpha\boldsymbol{v_1} + \beta\boldsymbol{v_2}) = \alpha L(\boldsymbol{v_1}) + \beta L(\boldsymbol{v_2})
$$则称其实为**线性变换(linear transformation)**. 记为$$L:V \to W$$


如果向量空间$$V$$和$$W$$是相同的，我们称线性变换$$L: V \to V$$为$$V$$上的**线性算子(linear operator)**.
'
[]




#### 4.1.1 从$$R^n$$到$$R^m$$的线性变换

一般地，如果$$A$$为任何$$m\times n$$矩阵，我们可定义一个从$$R^n$$到$$R^m$$的线性变换$$L_A$$，对于每一个$$\boldsymbol{x} \in R^n$$
$$
L_A(\boldsymbol{x}) = A\boldsymbol{x}
$$

#### 4.1.2 从$$V$$到$$W$$的线性变换

若$$L$$为一从向量空间$$V$$到$$W$$的线性变换，则
* $$L(\boldsymbol{0_v}) = \boldsymbol{0_w}$$
* 若$$\boldsymbol{v_1, \dotsc, v_n}$$为$$V$$的元素，且$$\alpha_1, \dotsc, \alpha_n$$为标题，则  
$$
L(\alpha_1\boldsymbol{v_1} + \alpha_2\boldsymbol{v_2} + \dotsb + \alpha_n\boldsymbol{v_n}) = \alpha_1L(\boldsymbol{v_1}) + \alpha_2L(\boldsymbol{v_2}) + \dotsb + \alpha_nL(\boldsymbol{v_n})
$$

* 对所有的$$\boldsymbol{v} \in V$$，有$$L(-\boldsymbol{v}) = -L(\boldsymbol{v})$$


#### 4.1.3 象与核

**定义** 令$$L: V \to W$$为一线性变换，$$L$$的**核(kernel)**记为$$ker(L)$$，定义为
$$
ker(L) = \{\boldsymbol{v} \in V \mid L(\boldsymbol{v}) = \boldsymbol(0_w)\}
$$
**定义** 令$$L: V \to W$$为一线性变换，并令$$S$$为$$V$$的一个子空间. $$S$$的**象(image)**记为$$L(S)$$，定义为
$$
L(S) = \{\boldsymbol{w} \in W \mid \boldsymbol{w} = L(\boldsymbol{v})，对某个 \boldsymbol{v} \in S\}
$$整个向量空间的象$$L(V)$$称为$$L$$的**值域(range)**.


**定理** 若$$L: V \to W$$为一线性变换，且$$S$$为$$V$$的子空间，则
* $$ker(L)$$为$$V$$的一个子空间
* $$L(S)$$为$$W$$的一个子空间


### 4.2 线性变换的矩阵表示

**定理** 若$$L$$为一从$$R^n$$到$$R^m$$的线性变换，则存在一个$$m\times n$$矩阵$$A$$，使得对每一个$$\boldsymbol{x} \in R^n$$，有
$$
L(\boldsymbol{x}) = A\boldsymbol{x}
$$



