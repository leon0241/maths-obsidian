**Tags:** #Algebra/Categories #Definition #Course/Category_Theory 

> [!Definition]+ Def: [[Definition of a Category]]
> 
> A category $C$ consists of 
> - A collection of *objects* $A,B,C, \dots$
> - A collection of *arrows* $f,g,h, \dots$
> - For each arrow, there are objects
> $$\dom(f),\,\quad \text{cod}(f)$$
> called the *domain* and *codomain* of $f$. We write
> $$f:A\to B$$
> to indicate that $A=\dom(f)$, and $B=\text{cod}(f)$.
> - Given arrows $f:A\to B$, and $g:B\to C$, that is, with
> $$\text{cod}{(f)}=\dom{(g)}$$
> there is given an arrow called the composite of $f$ and $g$
> $$g\circ f:A\to C$$
> - For each object $A$, there is given an arrow
> $$1_{A}:A\to A$$
> called the identity arrow of $A$ that satisfies the following axioms:
> 	- **Associativity:**
> 	$$h\circ (g\circ f) = (h\circ g) \circ f$$
> 	for all $f:A\to B$, $g:B\to C$, $h:C\to D$
> 	- **Identity:**
> 	$$f\circ 1_{A} = f = 1_{A} \circ f$$
> 	for all $f:A\to B$
^824748

%%EOF%%