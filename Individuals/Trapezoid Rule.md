**Tags:** #Python/Numpy #Definition #Course/CNU 

> [!Definition]+ Def: [[Trapezoid Rule]]
> 1. Choose nodes $x_{0}=-1, x_{1}=1$
> 2. With 2 nodes, the *interpolating polynomial* has degree 1
> 3. We therefore need the [[Quadrature Rules|quadrature rule]] to integrate degree-1 polynomials exactly i.e. to have [[Degree of Precision|degree of precision]] of at least 1
> 4. Use elementary polynomials of degree 0 and 1 to find the weights

$$\int_{-1}^{1}f(x)  \, dx ≈ \displaystyle\sum_{k=0}^{N-1} W_{k}f(x_{k)}$$
We need for $f(x)=p(x)=qx+l,\quad q,\,l\in\R,\quad \displaystyle\int_{-1}^{1} f(x) \, dx=\displaystyle\sum_{k=0}^{1}W_{k}f(x_{k})$
We need this to be true for $p(x)=1$ and $p(x)=x$
$p(x)=1$ (degree 0)
	$$\int_{-1}^{1} 1 \, dx =\displaystyle\sum_{k=0}^{1} W_{k} p(x_{k}) \implies 2 = W_{0}p(-1)+w_{1}p(1)=w_{0}+w_{1}$$
 $p(x)=x$ (degree 1)
	$$\int_{-1}^{1} x \, dx =w_{0}p(-1)+w_{1}p(1)\implies 0=-wp_{0}+w_{1}$$
	$$\implies w_{0}=w_{1}=1 \text{ is the weights for trapezoid rule}$$
$\implies$for arbitrary f(x), $\displaystyle\int_{-1}^{1} f(x) \, dx ≈ f(-1)+f(1)$
