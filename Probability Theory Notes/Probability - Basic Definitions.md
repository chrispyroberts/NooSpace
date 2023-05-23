---
dg-publish: true
---
## Random Experiments, Sample Spaces, and Events

**Definition:** [[Random Experiment]]
A random experiment is one for which:
1. All possible outcomes are known in advance.
2. Any performance of the experiment results in an outcome that is not known in advance.
3. The experiment can be repeated under identical conditions.

**Definition:** [[Sample Space]]
The sample space $S$ is the set of all possible outcomes of a random experiment
- Any element of S is a <u>sample point</u>.
- Any subset of S is called an <u>event</u>
- Any event which is a singleton is called a <u>simple event</u>
- Any event w/ cardinality $\ge 2$ is called a <u>compound event</u>

### Simple Example

A person tosses a coin. It lands on heads or tails.
$$S=\{H, T\}$$

**Definition:** [[Probability Measure]]
Given a sample space $S$, a probability measure is a frequency of $\mathbb{P}$, mapping events in $S$ to $\mathbb{R}$ such that it satisfies the following axioms:
1. $\mathbb{P}(A)\ge 0, \forall A\in S$
2. $\mathbb{P}(S)=1$
3. (Countable Additivity) For any sequence $A_{1,}A_{2,}... \subseteq S$, which is disjoint, then:
$$\mathbb{P}(\bigcup\limits_{i=1}^{\infty} A_{i)}= \sum\limits_{i=1}^{\infty}\mathbb{P}(A_i)$$

**Definition:** [[Finite Additivity]]
If $\mathbb{P}$ is a probability measure on $S$, then it is finitely additive. That is, for any disjoint events 
$$A_{1}, ... ,A_{n}$$
We have: 
$$\mathbb{P}(\bigcup\limits_{i=1}^{n}A_i)=\sum\limits_{i=1}^{n}\mathbb{P} (A_i)$$

**Strategy:** [[Turn any Finite Set into an Infinite Set]]
To turn a finite set of events into an infinite set of events, add on an infinite amount of empty sets onto the end of the finite set.

**Theorem:** [[Proporties of Probability Measures]]
Let $\mathbb{P}$ be a probability measure on a sample space S. Let $A,B\subseteq S$, then the following hold:
1. $\mathbb{P}(\emptyset) = 0$
2. $\mathbb{P}(A^{c})=1-\mathbb{P}(A)$
3. $A\subseteq B \implies \mathbb{P}(A)\le \mathbb{P}(B)$
4. $A\subseteq B \implies \mathbb{P}(B\backslash A) = \mathbb{P}(B)-\mathbb{P}(A)$
5. Finite Additivity as defined earlier: 
$$\mathbb{P}(\bigcup\limits_{i=1}^{n}A_i)=\sum\limits_{i=1}^{n}\mathbb{P} (A_i)$$


