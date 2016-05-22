### 1.3 矩阵算术

我们一般用$$\overrightarrow{x}$$表示**行向量(row vector)**，用加粗的小字母$$\boldsymbol{x}$$表示**列向量(column vector)**. 我们一般将列向量简称为向量.

**相等**

*定义* 若两个$$m \times n$$矩阵$$A$$和$$B$$对任一$$i$$和$$j$$均满足$$a_{ij} = b_{ij}$$，则称它们**相等(equal)**.

**标量乘法**

**定义** 若$$A$$为$$m \times n$$的矩阵，且$$\alpha$$为一标量，则$$\alpha A$$为一个$$m \times n$$的矩阵，其$$(i, j)$$元素为$$\alpha a_{ij}$$.

**矩阵加法**

**定义** 设$$A = (a_{ij})$$及$$B = (b_{ij})$$都是$$m \times n$$的矩阵，则它们的**和(sum)**$$A + B$$也为一个$$m \times n$$的矩阵，对每一个有序对$$(i, j)$$，它的(i, j)的元素为$$a_{ij} + b_{ij}$$.

**线性组合**

**定义** 若$$\boldsymbol{a_1, a_2, \dotsc, a_n}$$，为$$R^m$$中的向量，且$$c_1, c_2, \dotsc, c_n$$为标题，则和式
$$
c_1\boldsymbol{a_1} + c_2\boldsymbol{a_2} + \dotsb + c_n\boldsymbol{a_n}
$$
称为向量$$\boldsymbol{a_1, a_2, \dotsc, a_n}$$的一个**线性组合(linear combination)**.

** 矩阵乘法**

**定义** 若$$A = (a_{ij})$$为一个$$m \times n$$的矩阵，且$$B = (b_{ij})$$为一个$$n \times r$$的矩阵，则乘积$$AB = C = (c_{ij})$$为一个$$m \times r$$的矩阵，它的元素定义为
$$
c_{ij} = \boldsymbol{\overrightarrow{a_i}b_j} = \sum_{k = 1}^n a_{ik}b_{kj}
$$
