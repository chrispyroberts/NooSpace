---
dg-publish: true
---
Let $X$ be a [[Random Variable]]. The expected value (or expectation, or mean) of $X$ is denoted by $\mathbb{E}(X)$, and is defined as follows.

1. Suppose that $X$ is a [[Discrete Random Variable]] and has [[Probability Mass Function]] $p_{X}$. If $\sum\limits_{x}|x|p_{X}(x)\lt \infty$ then $\mathbb{E}(x)$ is said to exist and is defined by
$$\mathbb{E}(X)=\sum\limits_{x}xp_{X}(x)$$
  where the summation is taken over the support of $X$.

2. Supose that $X$ is a [[Continuous Random Variable]] and has [[Probability Density Function]] $f_{X}$. If $\int\limits_{-\infty}^{\infty}|x|f_{X}(x)dx\lt \infty$ then $\mathbb{E}(X)$ is said to exist, and is defined by
$$\mathbb{E}(X)=\int\limits_{-\infty}^{\infty}xf_{X}(x)dx$$
The expectation of a [[Discrete Random Variable]] can be interpreted as a weighted average of the elements of the support of $X$ with weights $p_{X}(x)$.

The expectation of a [[Continuous Random Variable]] is defined similarly as in the discrete case, by replacing the summation with an integral.
