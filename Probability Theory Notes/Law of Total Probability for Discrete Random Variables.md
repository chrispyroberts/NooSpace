---
dg-publish: true
---
**Remark:** [[Law of Total Probability for Discrete Random Variables]]
Suppose $X$ is a [[Discrete Random Variable]] with support $B=\{x_{1}, ..., x_{k}\}.$ Then the events $B_{i}={X=x_{i}}, \text{ for } i=1,...,k$ form a [[Partition]] of S.

![[Drawing 2023-05-25 20.04.53.excalidraw]]

This follows from the [[Law of Total Probability]]:
$$\mathbb{P}(A)=\sum\limits_{i=1}^{k}\mathbb{P}(A|B_{i})\mathbb{P}(B_{i})=\sum\limits_{i=1}^{k}\mathbb{P}(A|X=x_{i})p_X(x_{i})$$
