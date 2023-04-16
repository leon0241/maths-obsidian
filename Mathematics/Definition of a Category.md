**Tags:** #Algebra/Categories #Definition #Course/Category_Theory 

> [!Definition]+ Def: [[Definition of a Category]]
> 
> A category $\mathcal{C}$ consists of 
> - A collection $ob(\mathcal{C})$ of *objects*;
> - For each $A,B\in ob(\mathcal{C})$, a collection $\mathcal{C}(A,B)$ of *maps* or *arrows* or *morphisms* from $A$ to $B$
> - For each $A,B,C\in ob(\mathcal{C})$, a function
> $$\begin{align}
\mathcal{C}(B,C) \times \mathcal{C}(A,B) &\to \mathcal{C}(A,C) \\
(g,f) &\mapsto g\, \circ f
\end{align}$$
called *composition*
> - For each $A\in ob(\mathcal{C})$, an element $1_{A}$ of $\mathcal{C}(A,A)$ called the *identity* on $A$, satisfying the following axioms:
> 	- **associativity:** for each $f\in \mathcal{C}(A,B),\,g\in \mathcal{C}(B,C)$ and $h\in\mathcal{C}(C,D)$ we have $(h\circ g)\circ f = h\circ (g\circ f)$
> 	- **Identity** for each $f\in \mathcal{C}(A,B)$ we have $f\circ 1_{A} = f = 1_{B} \circ f$

^71e1c1
