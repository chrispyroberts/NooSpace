---
dg-publish: true
---
A random variable is supported on an interval $[a, b]$, and is equally likely to land in any sub-interval of $[a, b]$ of equal length. i.e. all values between $a$ and $b$ have equal probability density. In practice, the uniform distribution is used predominately for random number generation or for other simlation purposes.
![[Pasted image 20230602203205.png]]

**Properties:** [[Properties of Uniform Distribution]]
Notation: $X\sim \text{Unif}(a, b)$
Support: $[a, b]$
Parameters: $a:$ lower bound, $b:$ upper bound
PDF: 
$$f_{X}(x)=\begin{cases} \frac{1}{b-a}, & a\le x \le b \\ 0, & \text{otherwise}\end{cases}$$Expected Value: $\mathbb{E}[X]= \frac{a+b}{2}$
Variance: $\text{Var}[X]= \frac{(b-a)^{2}}{12}$

**Derivation:** [[Derivation of Expectation of Uniform Distribution]]
$$\displaylines{\mathbb{E}[X]=\int\limits_{-\infty}^{\infty}xf_{X}(x)dx =\int\limits_{a}^{b} \frac{x}{b-a}dx= \frac{1}{b-a}\bigg[\frac{x^{2}}{2}\bigg]^{b}_{a}= \\ \frac{1}{b-a}\bigg(\frac{b^{2}}{2}- \frac{a^{2}}{2}\bigg)=\frac{b^{2}-a^{2}}{2(b-a)}= \frac{a+b}{2}}$$
**Theorem:** [[The Probability Integral Transform]]
Suppose $F_{X}$ is a continuous CDF which is invertible $(\frac{dy}{dx}\ne 0,  \forall x\in \mathbb{R})$ over $\mathbb{R}$. Let $X\sim F_{X}$ and let $F_{X}^{-1}$ be the inverse of $F_{X}$. We have that:
$$ F_{X}(X)\sim U$$
and that 
$$F_{X}^{-1}(U)\sim F_{X}$$
The function $F_{X}^{-1}$ is called the quantile function of X


