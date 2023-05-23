---
dg-publish: true
---


**Definition:** [[Partition]]
A colection of events $\{B_{1},..., B_{k}\}\subseteq S$ is called a *partition* of the sample space $S$ if it satisfies the following: $$S=B_{1}\cup ... \cup B_{k} \text{ with } B_{i\cap}B_{j}=\emptyset \text{ for all } i\ne j.$$
Note that $B_i$ doesn't have to be a simple event. Assuming the elemtsn of the partition have positive probability, we can write down the probability of any event in $S$ in terms of its conditional probabilities given the elemnts of the partition; this is the law of total probability. 

**Theorem:** [[Law of Total Probability]]
Assume $\{B_{1}, ..., B_{k}\}$ is a partition of $S$. Assume that $\mathbb{P}(B_{i})\ge 0 \text{ for all } i$. Then, for any event $A\subseteq S$, it holds that: $$\mathbb{P}(A)=\sum\limits_{i=1}^{k}\mathbb{P}(A|B_{i})\mathbb{P}(B_{i}).$$
**Theorem:** [[Bayes' Rule]] 
Let $A, C$ be events in $S$, and $\{B_{1}, ..., B_{k}\}$ a partition of $S$. Suppose that $\mathbb{P}(A), \mathbb{P}(B_{i})\ge 0 \text{ for all } i=1,...,k$. Then, $$\mathbb{P}(C|A)=\frac{\mathbb{P}(A|C)\mathbb{P}(C)}{\mathbb{P}(A)}=\frac{\mathbb{P}(A|C)\mathbb{P}(C)}{\sum\limits_{i=1}^{k}\mathbb{P}(A|B_{i})\mathbb{P}(B_{i})}$$


