### 5.7 正交多项式

#### 正交序列

**定义** 若$$p_0(x),\, p_1(x),\, \dotsc$$为一多项式序列，且对每一个$$i$$有$$\deg{p_i(x)} = i. 若当 i \neq j$$时，$$\langle p_i(x), p_j(x)\rangle = 0$$，则$$\{p_n(x)\}$$称为**正交多项式序列(sequence of orthogonal polynomials)**. 若$$\langle p_i, p_j \rangle = \delta_{ij}$$，则$$\{p_n(x)\}$$称为**规范正交多项式序列(sequence of orthonormal polynomials)**


**定理** 若$$p_0, p_1, \dotsc$$为一正交多项式序列，则
* $$p_0, p_1, \dotsc, p_{n-1}$$构成了$$P_n$$的一组基
* $$p_n \in P_n^\bot$$(即$$p_n$$和每一次数小于$$n$$的多项式正交)

**定理** 令$$p_0, p_1, \dotsc$$为一正交多项式序列，对每一个$$i$$，令$$a_i$$表示$$p_i$$的首系数，并定义$$p_{-1}(x)$$为零多项式，则
$$
\alpha_{n+1}p_{n+1}(x) = (x - \beta_{n+1})p_n(x) - \alpha_n\gamma_np_{n-1}(x) \quad (n \geq 0)
$$其中$$\alpha_0 = \gamma_0 = 1$$，且
$$
\alpha_n = \frac{a_{n-1}}{a_n}, \quad \beta_n = \frac{\langle p_{n-1}, xp_{n-1}\rangle}{\langle p_{n-1}, p_{n-1}}, \quad \gamma_n = \frac{\langle p_n, p_n \rangle}{\langle p_{n-1}, p_{n-1}\rangle}\quad (n \geq 1)
$$
#### 经典正交多项式

**勒让德多项式**

勒让德多项式在内积
$$
\langle p, q \rangle  = \int_{-1}^1\,p(x)q(x)\mathrm{d}x
$$意义下正交，令$$P_n(x)$$表示次数为$$n$$的勒让德多项式，若选择首系数，使得对每一个$$n$$有$$P_n(1) = 1$$，则勒让德多项式的递推公式为
$$
(n + 1)P_{n+1}(x) = (2n + 1)xP_n(x) - nP_{n-1}(x)
$$利用这个公式，我们很容易得到一个勒让德多项式的序列，
$$
\begin{align}
P_0(x) &= 1 \\
P_1(x) &= x \\
P_2(x) &= \frac{1}{2}(3x^2 - 1) \\
P_3(x) &= \frac{1}{2}(5x^3 - 3x) \\
P_4(x) &= \frac{1}{8}(35x^4 - 30x^2 + 3)
\end{align}
$$
**切比雪夫多项式**

切比雪夫多项式在内积
$$
\langle p, q \rangle  = \int_{-1}^1\,p(x)q(x)(1 - x^2)^{-1/2}\mathrm{d}x
$$意义下正交，习惯上使用规范化的首系数，使得对$$k = 1, 2, \dotsc$$有$$a_0 = 1$$且$$a_k = 2^{k-1}$$，切比雪夫多莽同式记为$$T_n(x)$$，它有如下有趣的性质
$$
T_n(\cos{\theta}) = \cos{n\theta}
$$这个性质再加上三角恒等式
$$
\cos{(n + 1)\theta} = 2\cos{\theta}\cos{n\theta} - \cos{(n - 1)\theta}
$$可得到递推关系
$$
\begin{align}
T_1(x) &= xT_0(x) \\
T_{n + 1}(x) &= 2xT_n(x) - T_{n-1}(x), \quad n \geq 1
\end{align}
$$


