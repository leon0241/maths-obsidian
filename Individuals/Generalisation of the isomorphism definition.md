**Tags:** #Remark #Algebra/Categories #Course/Category_Theory  

> [!Remark]+ Def: [[Generalisation of the isomorphism definition]]
> The definition of [[Isomorphism#^9826ba|isomorphisms]] where
> $$g\circ f=1_{A}\quad\text{and} \quad f\circ g=1_{B}$$
> can be applied to any category. The definition that is commonly used between groups for example is one of a [[Functions#^6bb763|bijective]] function on the elements of the set. This is equivalent to the category theory definition, but it won't work in all cases. For example in the set of [[Poset#^900b1c|posets]] $\text{Pos}$, there are bijective [[Homomorphism#^f3e79f|homomorphisms]] between non-isomorphic posets. 
> One example is defined below:
> - Let $P=\{a,b,c\}$ where $a\le b$ and $a\le c$, but $b$ and $c$ aren't comparable. This is a valid poset from the 3 definitions.
> - Let $Q=\{x,y,z\}$ where $x\le y\le z$
> 
> Now let $f:P\to Q$ be defined by $a\mapsto x,\,b\mapsto y,\,c \mapsto z$. $f$ is bijective since you can map each element back, and since $x\le y$ and $x\le z$ it's a poset homomorphism. However, $g:Q\to P$ doesn't preserve the operations back so it isn't an isomorphism.

^209bcc

