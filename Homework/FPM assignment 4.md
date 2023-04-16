> [!Question]+ Question 1 [[FPM assignment 4|]]
> - a) Let $G$ and $H$ be two isomorphic finite groups and let $k$ be a postive integer. Prove that $G$ and $H$ have the same number of elements of order $k$
> - b) using part (a) or otherwise, prove that the groups $S_{4}$ and $D_{12}$ are not isomorphic

a) From Lemma 3.1.5, if $\phi:G\to H$ is injective, then the order of $g\in G$ equals the order of $\phi(g)\in H$. Since $\phi$ is an isomorphism, it is injective by definition. Therefore each element has the same order as its respective map, meaning $G$ and $H$ have the same number of elements of order $k$.

b) For the symmetric group $S_{4}$, an element can thought of as a cycle that maps up to $4$ elements in the set, for example the cycle that maps $0\mapsto 1,\,1\mapsto 2,\,2 \mapsto 3, 3\mapsto 0$ is represented like 
$$\left(\begin{matrix}
0&1&2&3 \\
1&2&3&0
\end{matrix}\right)$$
where the number of elements in the cycle will determine the order ($o(n)$) of the element, as after $n$ permutations an element returns back to its base state.
Elements with only one cycle have an order of the size of the element, while elements with multiple (disjoint) cycles have an order of the $\lcm$ of the orders of the two cycles as when one cycle returns to the base state it doesn't neccessarily guarantee the other cycle does as well.
- In $S_{4}$, the orders of single cycles can be in $\{1,2,3,4\}$, as there can only be up to 4 elements in a cycle. 
- Assuming any elements of the set that aren't counted are diregarded as $1$ doesn't affect the $\lcm$, there is only one combination for combinations of disjoint cycles that could have an order larger than a single cycle. This is an element of $o(2)$ paired with another element of $o(2)$, and it has an order of $2$.
- Therefore, the largest order of any element in $D_{4}$ is $4$.
In $D_{12}$ there exists an element of order $12$, namely the operation $g$ where $g$ is a rotation of $\frac{\pi}{6}$. After $12$ operations it's effectively a rotation of $2\pi$ which is the identity. 
However, since $S_{4}$ can't have an element of order $12$, this shows that $S_{4}$ and $D_{12}$ are not isomorphic by part (a), since there are a different amount of elements of order $12$ in the two groups.

> [!Question]+ Question 2
> Prove, using the $\epsilon-\delta$ definition of continuity that the function $f:\R\backslash\left\{ \frac{9}{5} \right\}\to \R$ defined by $f(x)=\displaystyle \frac{x^{2}}{5x-9}$ is continuous at $x_{0}=2$

**Proof:** Let $\epsilon>0$, and let $\delta=\min\left\{ 1, \frac{4}{15}\epsilon \right\}$. Then for any $x$ where $0<\lvert x-2 \rvert<\delta$,
$$\begin{align}
\lvert f(x)-f(a) \rvert  & = \left\lvert  \frac{x^{2}}{5x-9}-\frac{4}{10-9}  \right\rvert \\
&=\left\lvert  \frac{x^{2}}{5x-9}-4  \right\rvert \\
&=\left\lvert  \frac{x^{2}-20x+36}{5x-9}  \right\rvert \\
&=\left\lvert  \frac{(x-18)(x-2)}{5x-9}  \right\rvert  \\
&= \lvert x-2 \rvert \left\lvert  \frac{x-18}{5x-9}  \right\rvert \\
\end{align}
$$
- If we let the neighbourhood of $\delta$ around $x_{0}=2$ be no larger than $1$ (i.e. $\lvert x-2 \rvert< 1$), then we can get an upper bound of
$$\left\lvert  \frac{x-18}{5x-9}  \right\rvert < \left\lvert  \frac{3-18}{15-9}  \right\rvert=\left\lvert  \frac{-15}{4}  \right\rvert  \implies\quad \left\lvert  \frac{x-18}{5x-9}  \right\rvert  < \frac{15}{4}$$
Therefore,
$$\lvert x-2 \rvert \left\lvert  \frac{x-18}{5x-9}  \right\rvert < \lvert x-2 \rvert \cdot \frac{15}{4}$$
Therefore, since $0<\lvert x-2 \rvert < \delta$, and $\delta= \frac{4}{15}\epsilon$:
$$
\begin{align}
\lvert x-2 \rvert \cdot \frac{15}{4} &<\delta\cdot \frac{15}{4} \\
&= \frac{4}{15}\epsilon \cdot \frac{15}{4} \\
&=\epsilon
\end{align}$$
Therefore if $\delta= \frac{4}{15}\epsilon<1$, then $\lvert f(x)-f(a) \rvert = \lvert x-2 \rvert\left\lvert  \frac{x-18}{5x-9}  \right\rvert < \epsilon$.

- If $\delta\geq 1$, i.e. if $\epsilon>\frac{15}{4}$, then let $\delta=1$. Like above, this implies that $x<3$. Therefore:
$$
\begin{align}
\lvert x-2 \rvert \left\lvert  \frac{x-18}{5x-9}  \right\rvert&< 1\left\lvert  \frac{3-18}{15-9}  \right\rvert\\
&=\left\lvert  \frac{-15}{4} \right\rvert \\
&=\frac{15}{4} \le \epsilon
\end{align}
  $$

Therefore, for every $\epsilon>0$, if we choose $\delta=\min\left\{ 1, \frac{4}{15}\epsilon \right\}$ then we have
$$\lvert f(x) -f(a)\rvert<\epsilon $$
proving that the function is continuous at $x_{0}=2$