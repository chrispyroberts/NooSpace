---
dg-publish: true
---

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


