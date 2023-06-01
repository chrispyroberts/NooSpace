---
dg-publish: true
---
Suppose that we observe a sequence of independent trails which only have two possible outcomes, success or failure. We are interested in the number of trials until the first success occurs. 

Let $Y_{1},Y_{2}, ...$ be an infinite [[Bernoulli Process]]. So $Y_{i}\sim \text{Ber}(p)$ for some $p\in(0,1)$, and that the entire sequence is [[Independent]]. We are interested in finding the distribution of the random variable:
$$X=\text{min}\{k\ge1:Y_{k}=1\}$$
where $\text{min}\{k\ge1:Y_{k}=1\}$ is the smallest index $k$ for which the $k$-thj trial is a success. The distribution of $X$ is called a geometric distribution.

**Theorem:** [[Properties of Geometric Distribution]]
Notation:  $X\sim \text{Geom}(p)$
Support:  $\{1, 2,...\}$ or $\mathbb{N}$
Parameters:  $p:\text{ Sucess Probability}$
PMF:  $p_{X}(x)= p(1-p)^{x-1}$
Expected Value: $\mathbb{E}[X]= \frac{1}{p}$
Variance: $\text{Var}[X]= \frac{1-p}{p^{2}}$
