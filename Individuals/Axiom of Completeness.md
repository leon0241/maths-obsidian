**Tags:** #Main #Analysis/Reals #Course/FPM 

> [!Definition]+ Def: [[Axiom of Completeness]]
> If $E \subset \R$ is non-empty and bounded above, then $E$ has a supremum.

^5b377d

#### Idea
For the rational numbers $\Q$, if $q$ is rational then $\sqrt{q}$ isn't neccesarily rational. An example is $2$ and $\sqrt{ 2 }$. In other words, if q is rational, there may not be a rational number $x$ such that $x^2=q$.
The completeness axiom will fill in the gaps and ensure the reals include any number.

![[Bounds, Suprema and Infima#^35189a]]

#### Conceptualising the reals
The way we can think about completeness is that if we consider the set of rational numbers between $\pm \sqrt{ 2 }$, or
$$A := \{ x\in\Q: x^{2}<2 \}\quad \text{or} \quad A := \{ x\in\Q:0\le r \text{ and } r^{2}\le 2\}$$
- The set is bounded above (e.g $6$ or $2$ is larger than any element in the set)
- The least upper bound of the set is the smallest lower bound, or a number that's slightly larger than the infinitely closest rational value to $\sqrt{2}$, or in other words, $\sqrt{2}$ exactly.

If we start with $\Q$, and add in all the least upper bounds from every set that is bounded above, then we will include irrational numbers like $\sqrt{2}$ in our set. Doing this for every single set A will form a complete set of real numbers $\R$. This method of defining the axioms for $\R$ will also ensure that complex numbers like $3+2i$ are not included in the set

![[Least Upper Bound Property#^85a6f1]]

> [!Remark]+ Rem: [[Axiom of Completeness|Uniqueness of Suprema]]
> If a set has a supremum, it only has one supremum, i.e., the supremum is unique whenever it exists.

> [!Remark]+ Rem: [[Axiom of Completeness|Inclusion of Natural Suprema]]
> If $E\subset\N$ has a supremum, then $sup(E)\in E$

#### Consequences of completeness
![[Archimedean Principle#^7feff5]]

![[Density of the Rational Numbers#^800178]]
%%EOF%%