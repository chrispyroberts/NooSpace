Let $X, X_{1}, X_{2}$ all be discrete or continuous random variables. Let $a\in\mathbb{R}$. Then the following assertions hold.
1. $\mathbb{E}[aX]=a\mathbb{E}[X]$
2. $\mathbb{E}[a]=a$
3. $\mathbb{E}[X_{1}+X_{2}]=\mathbb{E}[X_{1}]+\mathbb{E}[X_{2}]$

Again, let $X$ be a random variable, and let $g:\mathbb{R}\rightarrow\mathbb{R}$ be a function. If the [[Expectation]] $g(X)$ exists, then it can be computed as follows:
$$\mathbb{E}[g(X)]=\begin{cases} 
      \sum\limits_{x}g(x)p_{X}(x), & X \text{ is discrete} \\
      \int\limits_{-\infty}^{\infty}g(x)f_{X}(x), & X \text{ is continuous} 
   \end{cases} $$
   