**Tags:** #Definition #Algebra/Categories #Course/Category_Theory 

> [!Definition]+ Def: [[Functor]]
> A functor
> $$F:C\to D$$
> between [[Definition of a Category#^824748|categories]] $C$ and $D$ is a mapping of objects to objects and arrows to arrows, in such a way that
> - $F(f:A\to B)=F(f):F(A)\to F(B)$
> - $F(1_{A})=1_{F(A)}$
> - $F(g\circ f)=F(g)\circ F(f)$

^c7347e

> [!Remark]+ Rem: [[Functor|Category Category]]
> Think of categories as objects, and functors as arrows. You can compose functors in the same way as any object, and each category $C$ has an identity functor $1_{C}:C\to C$.
> Therefore, we can construct the category of all categories and functors $\text{Cat}$

^e29f09

![[Category of Monoids#^63be0f]]