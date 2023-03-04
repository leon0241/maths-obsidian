**Tags:** #Algebra/Groups #Theorem #Course/FPM #TODO

> [!Theorem]+ Thm: [[Order of a finite group]]
> In a finite group, every element has finite order.

^291b9b

#### Proof
Let $g\in G$. Consider the inifinte sequence $g,g^2,g^3,\dots$ If $G$ is finite, then there must be repititions in this infinite sequence. Hence there exists $m,n\in\N$ with $m>n$ such that $g^m=g^n$. By cancelation, $g^{m-n}$ = e. This shows that $o(g)\le m-n$, and so consequently $o(g)$ is finite.