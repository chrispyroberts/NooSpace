---
dg-publish: true
---
### Definitions

**Definition:** [[Conditional Probability]]
Let $S$ be a sample space and $\mathbb{P}$ be a probability measure on $S$. Let $A, B\subseteq S$ such that $\mathbb{P}(B)\gt 0$ . The conditional probability of any event $A\subseteq S$ is given by: 
$$\mathbb{P}(A|B)=\frac{\mathbb{P}(A\cap B)}{\mathbb{P}(B)}$$
**Definition:** [[Independent]]
Given two events $A$ and $B$, we say that $A$ and $B$ are independent events if either of the following conditions hold:
1. $\mathbb{P}(A|B)=\mathbb{P}(A)$
2. $\mathbb{P}(B|A)=\mathbb{P}(B)$
3. $\mathbb{P}(A\cap B)=\mathbb{P}(A)\mathbb{P}(B)$

If a sequence $A_{1},..., A_{n}$ is *pairwise* independant if: 
$$\mathbb{P}(A_{i}\cap A_{j})=\mathbb{P}(A_{i})\mathbb{P}(A_{j}), \forall i\ne j$$
This tells us that: 
$$\mathbb{P}(\bigcap\limits_{i=1}^{n}A_{i})=\prod\limits_{i=1}^{n}A_i$$
### Useful Laws of Probability

**Theorem:** [[Multiplicative Law]]
The probability of the intersection of two events $A$ and $B$ is given by: 

$\hspace{2cm}\mathbb{P}(A\cap B)=\mathbb{P}(A)\mathbb{P}(B|A)=\mathbb{P}(B)\mathbb{P}(A|B)$
$\hspace{4.1cm}=0$ if $A$ and $B$ are disjoint
$\hspace{4.1cm}=\mathbb{P}(A)\mathbb{P}(B)$ if $A$ and $B$ are independant


**Theorem:** [[Additive Law]]
The probability of the union of two events $A$ and $B$ is given by:

$\hspace{2cm}\mathbb{P}(A\cup B)=\mathbb{P}(A)+\mathbb{P}(B)-\mathbb{P}(A\cap B)$
$\hspace{4.1cm}=\mathbb{P}(A)+\mathbb{P}(B)$ if $A$ and $B$ are disjoint
$\hspace{4.1cm}=\mathbb{P}(A)+\mathbb{P}(B)-\mathbb{P}(A)\mathbb{P}(B)$ if $A$ and $B$ are independant
