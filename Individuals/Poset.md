**Tags:** #Definition #TODO #Algebra/Categories #Course/Category_Theory 

> [!Definition]+ Def: [[Poset]]
> A partially ordered set, or a *poset* is a set $A$ equipped with a binary relation $a\le_{A} b$ such that the following conditions hold for all $a,b,c\in A$
> - **reflexivity:** $a\le_{A} a$,
> - **transitivity:** if $a\le_{A}b$ and $b\le_{A}c$, then $a\le_{A} c$
> - **antisymmetry:** if $a\le_{A} b$ and $b\le_{A} a$, then $a=b$
> 
> We can define an arrow from posets $A$ to $B$ as a function
> $$m:A\to B$$
> that is [[Monotone Sequences|monotone]], in the sense that for all $a,a'\in A$,
> $$a\le_{A} a'\text{ implies}\quad m(a)\le_{A}m(a')$$
> and from this, we have the category $\text{Pos}$ of posets and monotone functions

^900b1c

For posets to be categories, the other conditions must also be satisfied
- **Composition:** We need to know that if $f:A\to B$ and $g:B\to C$ are monotone, then $g\circ f:A\to C$ is also monotone. It follows that
$$a\le a' \implies f(a)\le f(a') \implies g(f(a))\le g(f(a'))\implies (g\circ f)(a)\le (g\circ f)(a')$$
- Identity?