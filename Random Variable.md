---
dg-publish: true
---
Let $S$ be a [[Sample Space]]. A random variable is a function of the form $X:S\rightarrow \mathbb{R}$.

**Example:**
$$S=\{(s_{1},...s_{50})|s_{i}\in [0, 100]\} \text{ is the sample space of student midterm grades }.
$$$$\mathbb{P}\left(\{(s_{1}, ..., s_{50}) | \frac{s_{1}+...+s_{50}}{50}\in [75, 90]\}\right)=\mathbb{P}(X\in [75, 90])$$

Where $X$ is the average of the class. So in this example, $$X((s_{1}, ..., s_{50}))=\frac{s_{1}+...+s_{50}}{50}$$
**Conventions:**
- $\forall B\subseteq \mathbb{R}, \{s\in S | X(s)\in B\}=\{X\in B\}$
- $\forall a\in \mathbb{R}, \{s\in S|X(s)\ge a\}=\{X\ge a\}$
- $\mathbb{P}(\{s\in S|X(s)\in B \text{ and } X(s)\ge x\})=\mathbb{P}(\{X\in B\}\cap \{X\ge x\}) =\mathbb{P}(X\in B, X\ge x))$

