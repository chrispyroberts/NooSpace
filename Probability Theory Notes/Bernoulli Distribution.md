---
dg-publish: true
---
A [[Random Variable]] X is said to follow a Bernoulli Distribution if its support is $\{0, 1\}$.  There must exist $p\in(0, 1)$ such that the PMF of $X$ satisfies:
$$p_{X}(1)=p, \hspace{1cm} p_{X}(0)=1-p$$

**Theorem:** [[Properties of Bernoulli Distribution]]
Notation:  $X\sim \text{Ber}(p)$
Support:  $\{0, 1\}$
Parameters:  $p:\text{Sucess Probability}$
PMF:  $p_{X}(x)=p^{x}(1-p)^{1-x} \hspace{1cm} x\in \{0, 1\}$
Expected Value: $\mathbb{E}[X]=p$
Variance: $\text{Var}[X]=p(1-p)$

**Definition:** [[Bernoulli Process]]
A Bernoulli Process is a sequence $X_{1}, ..., X_{n}$ of random variables such that for some $p\in(0, 1)$,
$$X_{i}\sim \text{Ber}(p), \hspace{1cm} i=1, ..., n$$
and such that $X_{1}, ..., X_{n}$ are [[Independent]].






