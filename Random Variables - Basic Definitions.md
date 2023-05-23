
### 2.1.2 Random Variables and their Distributions

**Definition:** [[Random Variable]]
Let $S$ be a [[Sample Space]]. A random variable is a function of the form $X:S\rightarrow \mathbb{R}$.

**Example:**
$$S=\{(s_{1},...s_{50})|s_{i}\in [0, 100]\} \text{ is the sample space of student midterm grades }.
$$$$\mathbb{P}\left(\{(s_{1}, ..., s_{50}) | \frac{s_{1}+...+s_{50}}{50}\in [75, 90]\}\right)=\mathbb{P}(X\in [75, 90])$$

Where $X$ is the average of the class. So in this example, $$X((s_{1}, ..., s_{50}))=\frac{s_{1}+...+s_{50}}{50}$$
**Conventions:**
- $\forall B\subseteq \mathbb{R}, \{s\in S | X(s)\in B\}=\{X\in B\}$
- $\forall a\in \mathbb{R}, \{s\in S|X(s)\ge a\}=\{X\ge a\}$
- $\mathbb{P}(\{s\in S|X(s)\in B \text{ and } X(s)\ge x\})=\mathbb{P}(\{X\in B\}\cap \{X\ge x\}) =\mathbb{P}(X\in B, X\ge x))$



**Definition:** [[Probability Distribution]]
Given a [[Random Variable]] $X:S\rightarrow \mathbb{R}$, its distribution is the function $P_X$ taking subsets $B\subseteq \mathbb{R}$ to $P_X(B)$ where: $$P_{X}(B)=\mathbb{P}(X\in B)=\mathbb{P}(\{s\in S|X(s)\in B\})$$

### 2.1.3 Cumulative Distribution Functions

**Definition:** [[Cumulative Distribution Function]]
Given a [[Random Variable]] $X$, its cumulative distribution function (CDF) is defined by: $$F_{X}:\mathbb{R}\rightarrow \mathbb{R}, F_{X}(x)=P_{X}((-\infty, x])=\mathbb{P}(X\le x)=\mathbb{P}(\{s\in S|X(s)\le x\})$$
A CDF measure the probability that a random variable will fall below a given point $x$. Such probabilities will arise frequently, which is the purpose of this notation.

**Proposition:** [[Special Case of CDF's Unique Characterization]]
Suppose that $X$ is a [[Random Variable]] with distribution $P_X$ and CDF $F_{X}$. Then, for all real numbers $a\lt b$, $$P_{X}((a, b])=\mathbb{P}(a\lt X \le b)=F_{X}(b)-F_{X}(a).$$
