---
dg-publish: true
---
### 2.3.1 The Expectation Operator

**Definition:** [[Expectation]] 
Let $X$ be a [[Random Variable]]. The expected value (or expectation, or mean) of $X$ is denoted by $\mathbb{E}(X)$, and is defined as follows.

1. Suppose that $X$ is a [[Discrete Random Variable]] and has [[Probability Mass Function]] $p_{X}$. If $\sum\limits_{x}|x|p_{X}(x)\lt \infty$ then $\mathbb{E}(x)$ is said to exist and is defined by
$$\mathbb{E}(X)=\sum\limits_{x}xp_{X}(x)$$
  where the summation is taken over the support of $X$.

2. Supose that $X$ is a [[Continuous Random Variable]] and has [[Probability Density Function]] $f_{X}$. If $\int\limits_{-\infty}^{\infty}|x|f_{X}(x)dx\lt \infty$ then $\mathbb{E}(X)$ is said to exist, and is defined by
$$\mathbb{E}(X)=\int\limits_{-\infty}^{\infty}xf_{X}(x)dx$$
The expectation of a [[Discrete Random Variable]] can be interpreted as a weighted average of the elements of the support of $X$ with weights $p_{X}(x)$.

The expectation of a [[Continuous Random Variable]] is defined similarly as in the discrete case, by replacing the summation with an integral.

### 2.3.2 Two Important Properties of Expectations

The [[Expectation]] is a "linear operator". The meaning of this is contained in the following theorem.

**Theorem:** [[Properties of Expectation Operators]]
Let $X, X_{1}, X_{2}$ all be discrete or continuous random variables. Let $a\in\mathbb{R}$. Then the following assertions hold.
1. $\mathbb{E}[aX]=a\mathbb{E}[X]$
2. $\mathbb{E}[a]=a$
3. $\mathbb{E}[X_{1}+X_{2}]=\mathbb{E}[X_{1}]+\mathbb{E}[X_{2}]$

Again, let $X$ be a random variable, and let $g:\mathbb{R}\rightarrow\mathbb{R}$ be a function. If the expectation $g(X)$ exists, then it can be computed as follows:
$$\mathbb{E}[g(X)]=\begin{cases} 
      \sum\limits_{x}g(x)p_{X}(x), & X \text{ is discrete} \\
      \int\limits_{-\infty}^{\infty}g(x)f_{X}(x), & X \text{ is continuous} 
   \end{cases} $$

**Definition:** [[Moment of a Random Variable]]
Let $j\in \mathbb{N}$ and $X$ a (discrete or continuous) random variable. We say that the j-th moment of $X$ exists (or that $X$ has finite j-th moment) if the [[Expectation]] of the random variable $X^j$ exists. In this case, the j-th moment of $X$ is given by $\mathbb{E}[X^j]$.

### 2.3.3 The Variance Operator

**Definition:** [[Variance]]
Let $X$ be a discrete or continuous random variable whose second moment exists. Then, its variance (or second central moment) is defined by
$$\text{Var}[X]=\mathbb{E}[(X-\mathbb{E}[X])^2]$$
Alternatively, the Variance can be expressed as follows:
$$\text{Var}[X]=E[X^2]-E[X]^2$$
The variance is a measure of spread or variability of the random variable $X$. It roughtly quantifies how much $X$ deviates from its center, on average.

It is important to note that the variance changes the units/scale of the problem as a result of squaring. The [[Standard Deviation]] fixes this problem by affixing a square root.

**Definition:** [[Standard Deviation]]
The standard deviation of a [[Random Variable]] $X$ is defined by
$$\sigma_{X}:=\sqrt{\text{Var}[X]}$$
where $\text{Var}[X]$ is the [[Variance]] of the random variable $X$.

**Proposition:** [[Proporties of Variance]]
Let $X$ be a [[Random Variable]] with finite second moment, and $a\in \mathbb{R}$. Then, 
1. $\text{Var}[X+a]=\text{Var}[X]$
2. $\text{Var}[a]=0$
3. $\text{Var}[aX]=a^2\text{Var}[X]$


### 2.4 Law of Total Probability for Random Variables

**Remark:** [[Law of Total Probability for Discrete Random Variables]]
Suppose $X$ is a [[Discrete Random Variable]] with support $B=\{x_{1}, ..., x_{k}\}.$ Then the events $B_{i}={X=x_{i}}, \text{ for } i=1,...,k$ form a [[Partition]] of S.

![[Drawing 2023-05-25 20.04.53.excalidraw]]

This follows from the [[Law of Total Probability]]:
$$\mathbb{P}(A)=\sum\limits_{i=1}^{k}\mathbb{P}(A|B_{i})\mathbb{P}(B_{i})=\sum\limits_{i=1}^{k}\mathbb{P}(A|X=x_{i})p_X(x_{i})$$
