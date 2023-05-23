---
dg-publish: true
---
The probbility mass function (PMF) of a [[Discrete Random Variable]] $X$ is defined by:
$$p_{X}(x)=\mathbb{P}(X=x), x\in \mathbb{R}$$
From this, we have:
$$P_{X}(B)=\sum\limits_{x\in B}p_{X}(x), \forall B\subseteq \mathbb{R}$$
This is a useful way to summarize the distribution of a discrete random variable.

Generally, if the support of $X$ is denoted $\chi$, and if $B\subseteq \mathbb{R}$, then we have the identity:
$$P_{X}(B)=\sum\limits_{b\in B\cap \chi}p_{X}(b)$$
which follows from Kolmogorov's third axiom. Since $p_{X}(y)=0$ for all $y\notin \chi ,$ we can also write the above expression as
$$P_{X}(B)=\sum\limits_{b\in B}p_{X}(b)$$We can deduce the following representation of the CDF for discrete random variables from this:
$$F_{X}(x)=\sum\limits_{y\le x}p_X(y)$$.