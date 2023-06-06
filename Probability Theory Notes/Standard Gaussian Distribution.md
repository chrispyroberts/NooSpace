---
dg-publish: true
---
When $\mu=0$ and $\sigma^{2}=1$, the distribution $N(\mu, \sigma^{2})$ is called the standard Gaussian distribution. We denote random variables from this distribution with the letter "$Z$", often writing $Z\sim N(0, 1)$. The CDF of such a random variable $Z$ has a distinguished notation:
$$\Phi(x)=F_{Z}(x)=\int\limits_{-\infty}^{x} \frac{1}{\sqrt{2\pi}}\exp\bigg( \frac{-y^{2}}{2}\bigg)dy, \hspace{1cm} x\in\mathbb{R}$$
The letter $\Phi$ will always be reserved for the CDF of the standard normal distribution.

From this, it follows that:
$$\mathbb{P}(a\le X \le b)=F_{X}(b)-F_{X}(a)=\Phi\bigg(\frac{b-\mu}{\sigma}\bigg)-\Phi\bigg(\frac{a-\mu}{\sigma}\bigg)$$
