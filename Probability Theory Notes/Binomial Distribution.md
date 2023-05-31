---
dg-publish: true
---
The binomial distribution is used to model [[Binomial Experiments]], which are experiments satisfying the following proporties:
- The experiment consists of the repetition of $n$ trials, where $n$ is fixed.
- Each trial has two possible outcomes: $1$ (success) or $0$ (failure).
- The probability of success remains $p$ throughout the experiment.
- Each trial is [[Independent]] of the others
- The [[Random Variable]] of interest is $X$, the total number of successes in $n$ trials.

You can represent the $n$ trials of a binomial experiment using a [[Bernoulli Process]]:
$$Y_{1},..., Y_{n}$$
This means that $Y_{i}\sim \text{Ber}(p)$ and $Y_{1}, ..., Y_{n}$ are independent. Think of $Y_{i}$ as representing the outcome of the $i$-th trial, so that $Y_{i}$ takes the value $1$ if the $i$-th trial is successful, and $0$ if unsuccessful. In this notation, the random variable of interest is:
$$X=\sum\limits_{i=1}^{n}Y_{i}$$
which represents the total number of successes across the $n$ trials. 

**Theorem:** [[Proporties of Binomial Distribution]]
Notation:  $X\sim \text{Bin}(n, p)$
Support:  $\{0, 1, ..., n\}$
Parameters:  $n: \text{ Number of Trials,}\hspace{1cm} p:\text{ Sucess Probability}$
PMF:  $p_{X}(x)= {n \choose x}p^{x}(1-p)^{n-x}, \hspace{1cm} x\in \{0, 1, ..., n\}$
Expected Value: $\mathbb{E}[X]=np$
Variance: $\text{Var}[X]=np(1-p)$
