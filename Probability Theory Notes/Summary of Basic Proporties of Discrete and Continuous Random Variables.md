---
dg-publish: true
---

|                                                     | Discrete                                                                                       | Continuous                                                                          |
| --------------------------------------------------- | ---------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- |
| Measure of Frequency                                | $\displaylines{\text{PMF }p_{X} \\ p_{X}(x)=\mathbb{P}(X=x)}$                                  | $\displaylines{\text{PDF } f_{X} \\ f_{X}(x)=F'_{X}(x)}$                            |
| Fundamental Proporties                              | $\displaylines{0\le p_{X}\le 1 \text{ for all } x\in \mathbb{R} \\ \sum\limits_{x}p_{X}(x)=1}$ | $\displaylines{0\le f_{X}(x) \text{ for all } x\in\mathbb{R} \\ \int f_{X}(x)dx=1}$ |
| Distribution $P_{X}(B)$ for $B\subseteq \mathbb{R}$ | $P_{X}(B)=\sum\limits_{y\in B}p_{X}(y)$                                                        | $P_{X}(B)=\int\limits_{B}f_{X}(y)dy$                                                |
| CDF $F_{X}(x)$ for $x\in\mathbb{R}$                 | $F_{X}(x)=\sum\limits_{y\le x}p_{X}(y)$                                                        | $F_{X}(x)=\int\limits_{-\infty}^{x}f_{X}(y)dy$                                      |
| $P_{X}((a,b])$                                      | $F_{X}(b)-F_{X}(a)$                                                                            | $F_{X}(b)-F_{X}(a)$                                                                 |
| $P_{X}([a, b])$                                     | $F_{X}(b)-F_{X}(a)+\mathbb{P}(X=a)$                                                            | $F_{X}(b)-F_{X}(a)$                                                                 |
                                                    |                                                                                                |                                                                                     |
