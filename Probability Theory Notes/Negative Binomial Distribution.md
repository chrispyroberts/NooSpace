---
dg-publish: true
---
Let $Y_{1}, Y_{2}, ...$ be an infinite [[Bernoulli Process]], where $Y_{i}\sim \text{Ber}(p)$ and $Y_i$ is independent of $Y_{j}$ for all $i\ne j$. We are interested in the random variable $X$ denoting the number of trials on whic hthe $r$-th success is observed.
$$X=min\Bigg\{K\ge1:\sum\limits_{i=1}^{k}Y_{i}=r\Bigg\}$$
In the special case where $r=1$, note that $X$ becomes a geometric random variable, but not when $r>1$. We write:
$$X\sim \text{NB}(r, p)$$
**Theorem:** [[Properties of Negative Binomial Distribution]]
Notation:  $X\sim \text{NB}(r, p)$
Support:  $\{r,r+1,...\}$
Parameters:  $r:\text{ Number of Successes,}\hspace{1cm} p:\text{ Sucess Probability}$
PMF:  $p_{X}(x)= {x-1 \choose r-1}p^{r}(1-p)^{x-r}, \hspace{1cm} r\le x$
Expected Value: $\mathbb{E}[X]= \frac{r}{p}$
Variance: $\text{Var}[X]= r\frac{1-p}{p^{2}}$
