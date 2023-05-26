Let $\mathbb{P}$ be a [[Probability Measure]] on a [[Sample Space]] $S$. Given a finite numbe of disjoint events $A_{1}, ..., A_{n}\subseteq S$ show that
$$\mathbb{P}(\bigcup\limits_{i=1}^{n}A_{i})=\sum\limits_{i=1}^{n}\mathbb{P}(A_{i})$$
Note that this merely differs from Kolmogorov's third axiom in the fact that the sequence of sets is finite rather than infinite.

**Proof:**
Define the infinite sequence of events
$$B_{i}= \left\{ \begin{array}{ll} A_{i},  \quad i\le n \\ \emptyset, \quad i\gt n \end{array} \right.$$
Since the $A_{i}$ are disjoint, and any set is disjoint from the empty set, the $B_i$ are disjoint. Thus, by Kolmogorov's third axiom, we have
$$\mathbb{P}(\bigcup\limits_{i=1}^{\infty}B_{i})=\sum\limits_{i=1}^{\infty}\mathbb{P}(B_{i})$$
Since $\mathbb{P}(\emptyset)=0$, from the proof that [[Probability of the Empty Set is 0]], the definition of $B_{i}$ implies that the right-hand side is equal to $\sum\limits_{i=1}^{n}\mathbb{P}(A_{i})$. Furthermore, notice that $\bigcup\limits_{i\gt n}B_{i}=\emptyset$ thus the left-hand side can be written as:
$$\mathbb{P}(\bigcup\limits_{i=1}^{\infty}B_{i})=\mathbb{P}(\bigcup\limits_{i=1}B_{i}\cup \emptyset)=\mathbb{P}(\bigcup\limits_{i=1}^{n}B_{i})=\mathbb{P}(\bigcup\limits_{i=1}^{n}A_{i})$$
The claim follows.
$\square$
[[Probability of the Empty Set is 0]]

