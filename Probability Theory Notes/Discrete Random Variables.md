---
dg-publish: true
---

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
which follows from Kolmogorov's third axiom. Since $p_{X}(y)=0$ for all $y\notin \chi ,$ we can also write the above expression as
$$P_{X}(B)=\sum\limits_{b\in B}p_{X}(b)$$We can deduce the following representation of the [[Cumulative Distribution Function]] for discrete random variables from this:
$$F_{X}(x)=\sum\limits_{y\le x}p_X(y)$$.
**Theorem:** [[Proporties of Probability Mass Functions]]
Let $X$ be a discrete random variable with support $\chi$. Let $p_X$ be the [[Probability Mass Function]] of $X$. Then:
1. $0\le p_{X}(x)\le 1,$ for all $x\in \mathbb{R}$
2. $\sum\limits_{x\in \chi}p_{X}(x)=1$

