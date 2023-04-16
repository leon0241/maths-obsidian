**Tags:** #Definition #Algebra/Categories #Course/Category_Theory 

> [!Definition]+ Def: [[Arrow Category]]
> The *arrow category* $\mathbf{C}^{\to}$ of a category $\mathbf{C}$ has the arrows of $\mathbf{C}$ as objects, and an arrow $g$ from $f:A\to B$ to $f':A'\to B'$ is a "commutative square"
> {img}
> where $g_{1}$ and $g_{2}$ are arrows in $\mathbf{C}$. That is, such an arrow is a pair of arrows $g=(g_{1},g_{2})$ in $\mathbf{C}$ such that
> $$g_{2}\circ f=f'\circ g_{1}$$
> The identity arrow $1_{f}$ on an object $f:A\to B$ is the pair $(1_{A}, 1_{B})$.
> Composition of arrows is done componentwise:
> $$(h_{1},h_{2})\circ (g_{1}, g_{2})=(h_{1}\circ g_{1},h_{2}\circ g_{2})$$
> There are two functors:
> $$\mathbf{C}\xleftarrow{\dom{}}\mathbf{C}^{\to}\xrightarrow{\text{cod}} \mathbf{C}$$