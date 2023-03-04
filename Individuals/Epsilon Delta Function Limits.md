**Tags:** #Definition #Analysis/Proofs #Course/FPM 

> [!Definition]+ Def: [[Epsilon Delta Function Limits]]
> Let $f:A\to\R$ and let $c$ be a limit point of $A$. Then we say that
> $$\displaystyle\lim_{x \to c} f(x) = L$$
> if for all $\epsilon>0$ there exists some $\delta>0$ such that for every $x\in A$ for which $0<\lvert x-c \rvert<\delta$, we have
> $$\lvert f(x)-L \rvert<\epsilon $$
> We also say $\displaystyle\lim_{x \to c}f(x)$ *converges* to L in such a situation

^e6f084

^87727d
> [!Remark]+ Rem: [[Epsilon Delta Function Limits|Domain Requirement]]
> The reason we require that $x\in A$ is just so that $f(x)$ makes sense, since $f:A\to R$, so if $x\not\in A$ then $f(x)$ is not even defined. (Note that we never take $f(c)$ so that's why it's ok if $c\not\in A$).

> [!Remark]+ Rem: [[Epsilon Delta Function Limits|Approach requirement]]
> The reason why we require $0<\lvert x-c \rvert$ (i.e. $x\ne c$) is because limits only care about what happens as you *approach* the point $c$, and not about what actually happens at the point $c$. $f(c)$ is able to not even be in the domain and the limit would be unaffected. For example, the chart below can still approach $\lim_{x \to 2}f(x)=1$ even if $f(2) \ne 1$
> ```tikz
> \begin{document}
> 	\begin{tikzpicture}[domain=0:4,scale=1.5]
> 		\draw[very thin,color=gray] (-0.1,-0.3) grid (4.2,2.5);
> 		\draw[->] (-0.2,0) -- (4.2,0) node[right] {$x$};
> 		\foreach \x in {1,2,3,4}
> 			\draw (\x cm,1pt) -- (\x cm,-1pt) node[anchor=north] {$\x$};
> 		\draw[->] (0,-0.3) -- (0,2.5) node[above] {$y$};
> 		\foreach \y in {1,2}
> 		    \draw (1pt,\y cm) -- (-1pt,\y cm) node[anchor=east] {$\y$};
> 		\draw[color=green]    plot (\x,\x/2)             node[right] {$f(x) $};
> 		\node[circle,draw, scale=0.7] (c) at (2,1){};
> 		\node[circle,fill,draw, scale=0.7] (c) at (2,2){};
> \end{tikzpicture}
> \end{document}
> ```

> [!Remark]+ Rem: [[Epsilon Delta Function Limits|Omittance of the first two conditions]]
> When the context is clear, for convenience we do not always explicitly state the conditions $x \in A$ and $0< \lvert x-c \rvert$.

> [!Remark]+ Rem: [[Epsilon Delta Function Limits|Visualising the epsilon delta limit]]
> For a fixed $\epsilon$ distance away from $L$, we want to find a $\delta$ such that the range of a fixed $\delta$ distance away from $c$ is contained within the range of $\epsilon$
> 
> ![[Pasted image 20230304182042.png]]
> We can also define uniform continuity as having a consistent $\delta$ for an $\epsilon$ on any point on a graph. You can see that if the point was moved to the left, the bounds for the size of $\delta$ would shrink. This is not covered on the course however, so it does not matter in this context.