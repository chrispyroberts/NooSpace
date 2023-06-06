---
dg-publish: true
---
Given a collection of random variables $Y_{1}, ..., Y_{n}$ we say they are i.i.d if they are [[Independent]] and [[Indentically Distributed]].

When $Y_{1},...,Y_{n}$ are i.i.d, and their equal distribution is given by $P_{Y}$, we write:
$$Y_{1}, ..., Y_{n}\mathop \sim \limits^{\text{i.i.d}}P_{Y}$$
Abusing notation, we may replace $P_{Y}$ on the right-hand side by $F_{Y}$, by $p_{Y}$ (in the discrete case) and $f_{Y}$ (in the continuous case).

As an example, if $Y_{1}, ..., Y_{n}$ form a Bernoulli process, then they are i.i.d., since they are independant and they each have the same distribution equal to $\text{Ber}(p)$ for some $p\in(0,1)$, we may then write:
$$Y_{1}, ..., Y_{n}\mathop \sim \limits^{\text{i.i.d}}\text{Ber}(p)$$
