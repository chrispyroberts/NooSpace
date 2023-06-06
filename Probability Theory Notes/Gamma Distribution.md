---
dg-publish: true
---
### 5.1.1 Generalities
The gamma distribution is a family of skew (i.e asymmetric) distributions used to model phenomena yielding non-negative random variables. For example, it can be used to model the time between events in a Poisson process, which cannot be negative.

A continuous random variable $X$ is said to follow a gamma distribution with parameters $\alpha, \beta \gt0,$ and $X\sim \text{Gamma}(\alpha, \beta)$, if its PDF takes the following form:
$$f_{X}(x)= \frac{x^{\alpha -1}e^{- \frac{x}{\beta}}}{\beta^{\alpha}\Gamma(\alpha)}, \hspace{0.5cm} x\ge 0$$
where $\Gamma$ denotes the [[Gamma Function]], defined by:
$$\Gamma(\alpha)=\int\limits_{0}^{\infty} y^{\alpha-1}e^{-y}dy, \hspace{0.5cm} \alpha\gt0$$
In the definition of a gamma distribution, the parameters $\alpha$ and $\beta$ are called the *shape* and *scale* parameters respectively. Increasing $\alpha$ drastically changes the qualitative shape of a gamma PDF, whereas increasing $\beta$ dilates it. This is illustrated in the following plots (taken from course notes):
![[Pasted image 20230606155447.png]]
When $\alpha$ is large relative to $\beta$, the shape of the gamma distribution is simualr to that of a [[Normal Distribution]]. IT can be shown that the $\text{Gamma}(\alpha, \beta)$ distribution approaches the $N(\alpha\beta, \alpha\beta^{2})$ distribution as $\alpha\rightarrow\infty$. 

Similarly to the Gaussian PDF, the antiderivative of the Gamma PDF is generally unavailable in closed form, thus you cannot compute probabilities for a Gama random variable without a computer or probability tables. The expection to this is if $\alpha$ is an integer, as then the antiderivative can be solved using integration by parts.

**Summary:** [[Properties of Gamma Distribution]]
Notation: $X\sim \text{Gamma}(\alpha, \beta) \text{ or } X\sim\Gamma(\alpha, \beta)$
Support: $[0, \infty)$
Parameters:  $\alpha\gt0:$ shape parameter, $\beta\gt0:$ scale parameter
PDF: 
$$f_{X}(x)= \frac{x^{\alpha-1}e^{- \frac{x}{\beta}}}{\beta^{\alpha}\Gamma(\alpha)},\hspace{0.5cm} x\ge0$$Expected Value: $\mathbb{E}[X]= \alpha\beta$
Variance: $\text{Var}[X]= \alpha\beta^{2}$

### **5.1.2** [[Exponential Distribution]]
When $\alpha=1$ and $\beta\gt0$, we can abbreviate the distribution $\Gamma(1, \beta)$ by $\text{Exp}(\beta)$, and we refer to it as the exponential distribution with parameter $\beta$. More generally, the distribution $\text{Gamma}(k, \beta)$ for $k\in\mathbb{N}$ is called an Erlang distribution, but we will mostly focus on the case where $k=1$.

**[[Exponential Distribution's Connection to Poisson Process]]:**
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
**[[Exponential Distribution's Connection to the Geometric Distribution]]:**
Both the exponential distribution and the geometric distribution measure the amount of time (or the number of trials) until the first occurance (or first success) is observed. Based on this connection, from the [[Memorylessness Properties of Geometric Distributions]], we also have the that exponential distribution is memoryless. 

It can be shown that any continuous memoryless distribution must be in the family of exponential distributions, in the same way that any discrete memoryless distribution must be in the family of geometric distributions. 

**Theorem:** [[Memorylessness Property of Exponential Distributions]]
Let $X\sim \text{Exp}(\beta)$. Then for all $a, b\gt 0:$
$$\mathbb{P}(X\gt a+b|X\gt a)=\mathbb{P}(X\gt b)$$

