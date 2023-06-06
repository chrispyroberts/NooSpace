---
dg-publish: true
---
Common examples of Poisson random variables:
- Let $X$ be the number of phone calls recieved by a person during one hour.
- Let $X$ be the number of motor accidents in an intersection per week.
- Let $X$ be the number of particle collisions in the collider per minute.
- Let $X$ be the number of decays from a radioactive sample per hour.

In general, the Poisson distribution is used to measure the number of occurances of an event over an interval of time. There are a few conditions on these occurances:

**Definition:** [[Poisson Process]]
1. Events occur independently of each other.
2. The rate of occurance of events is constant over the interval of time.
3. Events cannot occur simultaneously.

**Theorem:** [[Properties of Poisson Distribution]]
Notation:  $X\sim \text{Poisson}(p)$
Support:  $\{0, 1, ...\}$
Parameters: $\lambda : \text{Expected total number of events}$
PMF: $p_{X}(x)= \frac{\lambda^{x}e^{-\lambda}}{x!}$
Expected Value: $\mathbb{E}[X]= \lambda$
Variance: $\text{Var}[X]= \lambda$



