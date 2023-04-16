**Tags:** #Definition #Algebra/Categories #Course/Category_Theory #TODO 

> [!Definition]+ Def: [[Category of Monoids]]
> There is a [[Definition of a Category#^824748|category]] $\text{Mon}$ whose objects are [[Definition of a Monoid#^57cfb9|monoids]] and whose arrows are functions that preserve the monoid structure. In detail, a [[Homomorphism#^f3e79f|homomorphism]] from a monoid $M$ to a monoid $N$ is a function $h:M\to N$ such that for all $m,n\in M$,
> $$h(m\cdot_{M}n)=h(m)\cdot_{N}h(n)$$
> and $$h(u_{M})=u_{N}$$

^5c4ce6

> [!Remark]+ Rem: [[Category of Monoids|Monoids are Functors and Categories]]
> A monoid homomorphism from $M$ to $N$ is the same thing as a [[Functor#^c7347e|functor]] from $M$ regarded as a category, to $N$ regarded as a category. In this sense, categories are also generalised monoids, and functors are generalised homomorphisms.

^63be0f

> [!Example]+ [[Category of Monoids|Example:]] The set $\Z$ and $\N$
> Think of $\Z$ on the operation $+$ as a monoid, and the same for $\N$.
> Then a function $f:\mathbb{N}\to \Z$ such that for all $m,n\in \N$,
> $$f(m+_{\mathbb{N}}n)=f(m)+_{\mathbb{Z}}f(n)$$
> and
> $$f(1_{\mathbb{N}})=1_{\mathbb{Z}}$$
> is a valid arrow in the category $\text{Mon}$.
> However, since $\Z$ and $\N$ are monoids, they can be considered categories. From this a function $f:\mathbb{N}\to \Z$ can also be thought as a traversal between categories, or a functor.