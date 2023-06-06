---
dg-publish: true
---
Think of the hypergeometric distribution as taking the place of the [[Binomial Distribution]] when randomly sampling *without* replacement. 


The PMF of a hypergeometric random variable X is given as follows:
$$p_{X}(x)=\frac{{r\choose y}{N-r \choose n-y}}{{N\choose n}} \hspace{1cm} 0\le x\le n, \text{ such that } x\le r \text{ and }n-x\le N-r$$
**Derivation:** 
$$\mathbb{P}(X=x)=\frac{\text{ \# ways selecting } x \text{ successes AND } n-x \text{ failures}}{\text{\# ways of selecting }n\text{ objects}}$$
We have:
- The number of ways of selecting $n$ objects out of $N$ is $N \choose n$
- The number of ways of selecting $x$ successes among the $r$ total successes in the population is $N-r \choose n-x$
- The number of ways of selecting $n-x$ failures among the $N-r$ total failures in the population is $N-r\choose n-x$

Hence, we get:
$$\mathbb{P}(X=x)=\frac{{r\choose y}{N-r \choose n-y}}{{N\choose n}}$$

**Theorem:** [[Properties of Hypergeometric Distribution]]
Notation:  $X\sim \text{HG}(r, N, n)$
Support:  $\{x\in \mathbb{N}\cup \{0\}: 0\le x \le n, x\le r, n-x\le N-r\}$
Parameters:  $r:\text{ Number of Successes in Population}$
$\hspace{2.6cm} N:\text{ Population Size}$
$\hspace{2.6cm} n: \text{ Number of Trials}$
PMF: $p_{X}(x)=\frac{{r\choose x}{N-r \choose n-x}}{{N\choose n}}$
Expected Value: $\mathbb{E}[X]= \frac{nr}{N}$
Variance: $\text{Var}[X]= \frac{nr}{N} \frac{N-r}{N}\frac{N-n}{N-1}$

