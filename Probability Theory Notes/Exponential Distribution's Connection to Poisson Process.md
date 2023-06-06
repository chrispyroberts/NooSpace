---
dg-publish: true
---
The exponential distribution plays an important role in probability, since it is the distribution of the time difference between successive events in a [[Poisson Process]], with an appropriate rate parameter. Similarly, the Erlang distribution is the distribution of the time between $k$ events of a Poisson process. It is nontrvial to prove these facts, and we won't study them formally. That being said, the following identity will hint at these connections.

**Theorem:** 
Suppose $X\sim\text{Gamma}(k, \frac{1}{\lambda})$ and $N\sim\text{Po}(T\lambda),$ for some $k\in\mathbb{N}$ and $T, \lambda, \gt0$. Then:
$$\mathbb{P}(N\lt k)=\mathbb{P}(X\gt T)$$
This is better explained in plain English. Suppose that the occurance of certain events follows a Poisson process. Let $N$ be the number of occurances that take place between time $0$ and some time $T$, and let $T\lambda$ denote the expected number of occurances within the interval $[0, T]$. Let $X$ be the time until the $k$-th occurance of the Poisson process takes place. Then, this theorem is saying that the probabilities of the following two events are equal:
1. The number of occurances $N$ within the time interval $[0, T]$ is less than $k$.
2. The waiting-time $X$ until the $k$-th occurane is greater than $T$.

It should be intuitive that these events are describing the same thing. The theorem is showing that the Erlang distribution $\text{Gamma}(k, \frac{1}{\lambda})$ is the appropriate distribution to place on $X$ in order for these events to have equal probability.

Note that if $X\sim\text{Gamma}(k, 1)$ is an Erlang random variable representing the waiting time until the $k$-th occurance of an event in a Poisson process, then we can decompose $X$ as:
$$X=\sum\limits_{i=1}^{k}Y_{i}$$
where $Y_{i}$ is the waiting time between the $(i-1)$-th and $i$-th event of the Poisson process. Since the events of a Poisson process occur at a constant rate over time, and independently of one another, it is reasonable to expect that the random variables $Y_{i}$ are independent and identical distributions. ([[i.i.d]]) Furthermore, we know that $Y_{1}$ is just the waiting time until the first occurance, which has distribution $\text{Exp}(1)$. Therefore, the above display suggests that the sum of $k$ i.i.d. exponential random variables is distributed as an Erlang distribution with shape parameter $k$. This can also be generalized to the case where $k$ is not an integer. The result is stated in the following theorem.

**Theorem:**
Suppose $Y_{1}, ..., Y_{n}\mathop \sim \limits^{\text{i.i.d}}\text{Gamma}(\alpha, \beta)$ for some $\alpha,\beta\gt0$. Then:
$$\sum\limits_{i=1}^{k}Y_{i}\sim \text{Gamma}(k\alpha,\beta)$$