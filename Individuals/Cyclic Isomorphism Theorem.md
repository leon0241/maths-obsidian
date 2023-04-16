**Tags:** #Theorem 

> [!Theorem]+ Thm: [[Cyclic Isomorphism Theorem]]
> - All finite [[Cyclic Subgroups|cyclic groups]] of the same order are [[Isomorphism#^8c41ad|isomorphic]] to each other.
> - All infinite cyclic groups are isomorphic to each other.

^f7cc2d

#### Proof
Let $G$ and $H$ be two cyclic groups of order $n$. Write $G=\langle g \rangle = \{e,g, \dots g^{n-1}\}$ and $H=\langle h \rangle=\{e,h, \dots, h^{n-1}\}$, where $o(g)=n,o(h)=n$
Define $\phi:G\to H$ by $\phi(g^k)=h^k$ for $k=0,1,\dots,n-1$
- $\phi$ is a surjection
- $\phi$ is an injection: if $\phi(g^k)=\phi(g^l)$ (which would mean it isn't one-to-one) for some $k,l$ with $0\le k,l\le n-1$, then $h^k=h^l \implies\quad k=l, \implies\quad g^k=g^l$

Therefore $\phi$ is a bijection. Now we need to show $\phi$ is a homomorphism
For all $k,l$ with $0\le k,l\le n-1$ we have
$$\phi(g^kg^l)=\phi(g^{k+l})=h^{k+l}=h^kh^l=\phi(g^k)\phi(g^l)$$
where $+$ is addition mod $n$. Therefore from this $G$ and $H$ are isomorphisms