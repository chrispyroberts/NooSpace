---
dg-publish: true
---
Let $X$ be a random variable, and let $g:\mathbb{R}\rightarrow\mathbb{R}$ be a function. If the [[Expectation]] $g(X)$ exists, then it can be computed as follows:
$$\mathbb{E}[g(X)]=\begin{cases} 
      \sum\limits_{x}g(x)p_{X}(x), & X \text{ is discrete} \\
      \int\limits_{-\infty}^{\infty}g(x)f_{X}(x), & X \text{ is continuous} 
   \end{cases} $$
   