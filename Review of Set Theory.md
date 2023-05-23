
### Basic Definitions

**Definition:** [[Set]]
A *set* is an unordered collection of objects.
$$\{1, 2, 3, 4, 5, 6, 7\} = \{7, 6, 5, 4, 3, 2, 1\}$$
Another way of expressing this set is the following:
$$\{i: i\text{ is an integer and } i\le i \le 6 \}$$
or
$$\{1\le i \le 6 : i \text{ is an integer}\}$$
When we want to talk about ordered collections of objects, we will prefer to use round brackets, and we will refer to them as **tuples**.
$$(1, 2, 3, 4, 5, 6)\neq(6, 5, 4, 3, 2, 1)$$
###### Example 1.
There are some common mathematical sets with distinguished notation
- $\mathbb{N}$ :The set of (posititive) natural numbers.
- $\mathbb{Z}$: The set of (possibly negative) integers.
- $\mathbb{R}$: The set of real numbers, sometimes denotes as the interval $(-\infty, \infty)$
- $\mathbb{R}^2$: The two-dimensional plane. $\mathbb{R}^{2}= \{(x, y): x, y \in \mathbb{R}\}$

### Set Operations

**Definition:** [[Set Operations]]
| Term | Notation | Intuitive Terminology | Precise Definition |
| --- | --- | --- | --- |
| Superset | $A\supseteq B$ | "encompasses" | $A\supseteq B$ means $\forall x \in B, x \in A$
| Subset | $A\subseteq B$ | "within" | $A\subseteq B$ means $\forall x \in A, x \in B$
| Strict Superset | $A\supsetneq B$ | "strictly encompasses" | $A\supsetneq B$ means $A\supseteq B$ AND $A\neq B$
| Strict Subset | $A\subsetneq B$ | "strictly within" | $A\subsetneq B$ means $A\subseteq B$ AND $A\neq B$
| Union | $A\cup B$ | "or" | $A\cup B =  \{x: x \in A \text{ OR } x \in B\}$
| Intersection | $A\cap B$ | "and" | $A\cap B = \{x: x\in A \text{ AND } x\in B\}$
| Difference | $A\backslash B$ | "except" | $A\backslash B = \{x: x\in A, x\notin B\}$
| Complement | $A^c$ | "not" | $A^{c} = S\backslash A$ (*S depends on the application of the complement*)

### More notation and definitions

**Definition:** [[Cardinality]] 
The size as cardinality of a set A is |A|.

**Definition:** [[Empty Set]]
$\emptyset =  \{ \}, |\emptyset | = 0$

**Definition:** [[Singleton]]
A is a singleton if |A| = 1

**Definition:** [[Union & Intersection of an Infinite Sequence]]
Let $A_{1,}A_{2,}...$ be a sequence of sets.
- $\bigcup\limits_{n=1}^{\infty} A_{i} = A_{1}\cup A_{2}\cup ... = \{x: \text{ there exists } i \text{ s.t } x\in A_i\}$
- $\bigcap\limits_{n=1}^{\infty} A_{i} = A_{1}\cap A_{2}\cap ... = \{x: \text{ for all } i \text{ s.t } x\in A_i\}$

**Definition:** [[Basic Propositions]]
Let $A, B, C \subseteq S$
1. $A\cup A^{c}=S$
2. [[Associativity]]: $(A\cap B)\cap C = A\cap B \cap C$
3. [[Distributivity]] $A\cap (B\cup C) = (A\cap B) \cup (A\cap C)$
4. [[De Morgan's Laws]]
	1.  $(A\cap B)^{c}= A^{c}\cup B^c$
	2. $(A\cup B)^{c}= A^{c}\cap B^c$
5. [[Disjoint]] A and B are disjoint if $A\cap B = \emptyset$

### Some basic exercises
Let $A, B \subseteq C$. Using only identities $A=A\cap S$ and $S = B\cup B^c$, and above propositions, prove the following:

1. $A = (A\cap B)\cup (A\cap B^c)$
	We know $A=A\cap S$ and S = $B\cup B^{c}$, so $A=A\cap(B\cup B^c)$, then by distribuitivity, we can see that $A=(A\cap B) \cup (A\cap B^c)$. 

2. If $B\subseteq A$, then $A=B\cup (A\cap B^c)$
	Since B is a subset of A, then by definition of $\subseteq$: $$B=B\cap A$$Then substituting into the result from 1:$$\displaylines{A=(A\cap B) \cup (A\cap B^{c}) \\ A = B\cup (A\cap B^c)}$$
3. Show that $A\cap B$ and $A\cap B^c$ are disjoint.
	By the Distributivity Property, $(A\cap B) \cap (A \cap B^{c}) = A\cap B \cap B^{c}$.
	Since $B\cap B^{c}=\emptyset$, then $A\cap B \cap B^{c}= A\cap \emptyset = \emptyset$.
	
4. Show that $B$ and $A\cap B^c$ are disjoint.
	By distributivity property, $B\cap (A\cap B^{c}) = B\cap B^{c}\cap A = \emptyset \cap A = \emptyset$
 
