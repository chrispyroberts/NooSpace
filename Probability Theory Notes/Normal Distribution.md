---
dg-publish: true
---
The importance of the normal distribution stems primarily from three facts:
1. The observed data of many physical phenomena are at least approximately normal.
2. It is the 'limiting distribution' of other distributions that we will encounter.
3. It figures prominetly in the [[Central Limit Theorem]]. 

A continuous random variable $X$ is Gaussian or normally distributed if its PDF takes the following form:
$$f_{X}(x)=\frac{1}{\sqrt{2\pi \sigma^{2}}}\exp\bigg(-\frac{(x-\mu)^{2}}{2\sigma^{2}}\bigg), x\in\mathbb{R}$$
Here, $\mu\in\mathbb{R}$ and $\sigma^{2}\gt0$ are parameters of the Gaussian distribution. We will shortly see that they respectively denote the mean and variance of $X$. We write $X\sim N(\mu, \sigma^{2})$.

**Proporties**: [[Properties of Normal Distributions]]
Notation: $X\sim N(\mu, \sigma^{2})$
Support: $\mathbb{R}$
Parameters: $\mu:$ Mean,  $\sigma^{2}:$ Variance
PDF: 
$$f_{X}(x)=\frac{1}{\sqrt{2\pi \sigma^{2}}}\exp\bigg(-\frac{(x-\mu)^{2}}{2\sigma^{2}}\bigg), x\in\mathbb{R}$$Expected Value: $\mathbb{E}[X]= \mu$
Variance: $\text{Var}[X]= \sigma^{2}$

**Remark:** [[Standard Gaussian Distribution]]
When $\mu=0$ and $\sigma^{2}=1$, the distribution $N(\mu, \sigma^{2})$ is called the standard Gaussian distribution. We denote random variables from this distribution with the letter "$Z$", often writing $Z\sim N(0, 1)$. The CDF of such a random variable $Z$ has a distinguished notation:
$$\Phi(x)=F_{Z}(x)=\int\limits_{-\infty}^{x} \frac{1}{\sqrt{2\pi}}\exp\bigg( \frac{-y^{2}}{2}\bigg)dy, \hspace{1cm} x\in\mathbb{R}$$
The letter $\Phi$ will always be reserved for the CDF of the standard normal distribution.

From this, it follows that:
$$\mathbb{P}(a\le X \le b)=F_{X}(b)-F_{X}(a)=\Phi\bigg(\frac{b-\mu}{\sigma}\bigg)-\Phi\bigg(\frac{a-\mu}{\sigma}\bigg)$$
**Proposition:** [[Symmetric Distributions]]
Once we know the values of $\Phi(x)$ for $x\ge 0$, we also know them for all $x\lt0$, since the standard Gaussian PDF is symmetric around 0.

Suppose that $Y$ is a continuous random variable whose PDF $f_{Y}$ is an [[Even Function]] for all $y\in\mathbb{R}$. In this case, $Y$ has a symmetric distribution, and its CDF satisfies the relation:
$$F_{Y}(y)=1-F_{Y}(-y), \hspace{1cm} y\in\mathbb{R}$$
