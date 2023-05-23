---
dg-publish: true
---
Given two events $A$ and $B$, we say that $A$ and $B$ are independant events if either of the following conditions hold:
1. $\mathbb{P}(A|B)=\mathbb{P}(A)$
2. $\mathbb{P}(B|A)=\mathbb{P}(B)$
3. $\mathbb{P}(A\cap B)=\mathbb{P}(A)\mathbb{P}(B)$

If a sequence $A_{1},..., A_{n}$ is *pairwise* independant if: 
$$\mathbb{P}(A_{i}\cap A_{j})=\mathbb{P}(A_{i})\mathbb{P}(A_{j}), \forall i\ne j$$
This tells us that: 
$$\mathbb{P}(\bigcap\limits_{i=1}^{n}A_{i})=\prod\limits_{i=1}^{n}A_i$$