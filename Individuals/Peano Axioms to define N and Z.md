**Tags:** #Definition #Analysis/Reals  #Course/FPM 

> [!Definition]+ Def: [[Peano Axioms to define N and Z]]
> From just stating $N = \{1,2,3,\dots\}$, it is not clear what $2$ or $3$ actually is, so we will need to define $2$ as $1 + 1$, and $3$ as $2 + 1$ or $1 + 1+1$, and so forth. Define functions $s(n)$(successor of $n$) and $p(n)$(predecessor of $n$) where $s(n)=n+1$, and $p(n) = n - 1$. We can first construct a list of axioms to define every number in $\N_0$ called the Peano Axioms.
> - **N1:** $0\in\N_0$
> - **N2:** For any $n\in\N_0$, there exists $s(n)\in\N_0$
> - **N3:** If $s(n) = s(m)$ then $n = m$
> - **N4:** There does not exist $n\in\N_0$ with $s(n) = 0$
> - **N5:** If $0\in A\subset\N$ and if $n\in A$ implies $s(n)\in A$ then $A = \N_0$
> 
 We can then define $\Z$ as a set that contains $\N_0$ and has the following properties:
> - **Z1:** Given $n\in\Z$ then there exists $p(n)\in\Z$ such that $s(p(n))=n$
> - **Z2:** If $A\subset\Z$ and $s(n)\in A$ iff $n\in A$, then $A = Z$

^2442a6


%%EOF%%