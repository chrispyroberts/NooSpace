---
dg-publish: true
---

### 2.2.1 Discrete Random Variables

**Definition:** [[Support of a Random Variable]]
The Support of a [[Random Variable]] is the "smallest" set of $B$ such that $P_{X}(B)=1$.

**Definition:** [[Countable Set]]
A set is countable if it is finite or if it is infinite but in 1-to-1 correspondance with the Natural Numbers ($\mathbb{N}$).

**Definition:** [[Discrete Random Variable]]
A [[Random Variable]] is said to be discrete if its Support is a [[Countable Set]].

**Definition:** [[Probability Mass Function]]
The probbility mass function (PMF) of a [[Discrete Random Variable]] $X$ is defined by:
$$p_{X}(x)=\mathbb{P}(X=x), x\in \mathbb{R}$$
From this, we have:
$$P_{X}(B)=\sum\limits_{x\in B}p_{X}(x), \forall B\subseteq \mathbb{R}$$
This is a useful way to summarize the distribution of a discrete random variable.


Generally, if the support of $X$ is denoted $\chi$, and if $B\subseteq \mathbb{R}$, then we have the identity:
$$P_{X}(B)=\sum\limits_{b\in B\cap \chi}p_{X}(b)$$
This follows from Kolmogorov's third axiom. Since $p_{X}(y)=0$ for all $y\notin \chi ,$ we can also write the above expression as
$$P_{X}(B)=\sum\limits_{b\in B}p_{X}(b)$$
We can deduce the following representation of the [[Cumulative Distribution Function]] for discrete random variables from this:
$$F_{X}(x)=\sum\limits_{y\le x}p_X(y)$$

In summary, the PMF of a random variable $X$ is a way to illustrate the relative frequency with which we expect to see any value of $X$ occur.

**Theorem:** [[Proporties of Probability Mass Functions]]
Let $X$ be a discrete random variable with support $\chi$. Let $p_X$ be the [[Probability Mass Function]] of $X$. Then:
1. $0\le p_{X}(x)\le 1,$ for all $x\in \mathbb{R}$
2. $\sum\limits_{x\in \chi}p_{X}(x)=1$

### 2.2.2 Continuous Random Variables

**Definition:** [[Continuous Random Variable]]
A [[Random Variable]] $X$ is said to be continuous if its [[Cumulative Distribution Function]] $F_{X}$ is a continuous function over $\mathbb{R}$. 

Given any continuous random variable $X$, it holds for all $x\in \mathbb{R}$ that $\mathbb{P}(X=x)=0$

**Definition:** [[Probability Density Function]]
Let $X$ be a continuous random variable with [[Cumulative Distribution Function]] $F_X$. The probability density function (PDF) of $X$ is defined by
$$f_{X}(x)=F'_{X}(x)=\frac{dF_{X}(x)}{dx}$$
for all $x\in\mathbb{R}$ where the derivative $F_{X}$ exists.

By the Fundamental Theorem of Calculus, this definition implies that we can write
$$F_{X}(x)=\int\limits_{-\infty}^{x}f_{X}(y)dy$$
for all $x\in\mathbb{R}$. Furthermore, recalling [[CDF on an Interval]], we can also write
$$P_{X}((a, b])=\int\limits_{a}^{b}f_{X}(y)dy=P_{X}([a, b])=P_{X}([a, b))=P_{X}((a, b))$$
where the second, third, and fourth equalities follow from the fact that $P_{X}(\{a\})=P_{X}(\{b\})=0$ for a [[Continuous Random Variable]], and Kolmogorov's third axiom. More generally, if $B\subseteq \mathbb{R}$ is a general set, we can express the distribution of $X$ as an integral over this region of integration:
$$P_{X}(B)=\int\limits_{B}f_{X}(y)dy$$
In summary, we will typically compute probabilities for random variables by integrating PDFs, rather than summing PMFs as we do for discrete random variables.

**Theorem:** [[Fundamental Proporties of Probability Distribution Functions]]
Let $X$ be a [[Continuous Random Variable]] with [[Probability Density Function]] $f_X$. Then,
1. $0\le f_{X}(x)$ for all $x\in\mathbb{R}$.
2. $\int\limits_{-\infty}^{\infty}f_{X}(x)dx=1$

Notice that PDFs do not need to be bounded above by 1, unlike PMFs.

### 2.2.3 Summary

This is alot of proporties about discrete and continuous random variables. Here is a summary of them in a table:

**Table:**  [[Summary of Basic Proporties of Discrete and Continuous Random Variables]]

|                                                     | Discrete                                                                                       | Continuous                                                                          |
| --------------------------------------------------- | ---------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- |
| Measure of Frequency                                | $\displaylines{\text{PMF }p_{X} \\ p_{X}(x)=\mathbb{P}(X=x)}$                                  | $\displaylines{\text{PDF } f_{X} \\ f_{X}(x)=F'_{X}(x)}$                            |
| Fundamental Proporties                              | $\displaylines{0\le p_{X}\le 1 \text{ for all } x\in \mathbb{R} \\ \sum\limits_{x}p_{X}(x)=1}$ | $\displaylines{0\le f_{X}(x) \text{ for all } x\in\mathbb{R} \\ \int f_{X}(x)dx=1}$ |
| Distribution $P_{X}(B)$ for $B\subseteq \mathbb{R}$ | $P_{X}(B)=\sum\limits_{y\in B}p_{X}(y)$                                                        | $P_{X}(B)=\int\limits_{B}f_{X}(y)dy$                                                |
| CDF $F_{X}(x)$ for $x\in\mathbb{R}$                 | $F_{X}(x)=\sum\limits_{y\le x}p_{X}(y)$                                                        | $F_{X}(x)=\int\limits_{-\infty}^{x}f_{X}(y)dy$                                      |
| $P_{X}((a,b])$                                      | $F_{X}(b)-F_{X}(a)$                                                                            | $F_{X}(b)-F_{X}(a)$                                                                 |
| $P_{X}([a, b])$                                     | $F_{X}(b)-F_{X}(a)+\mathbb{P}(X=a)$                                                            | $F_{X}(b)-F_{X}(a)$                                                                 |



