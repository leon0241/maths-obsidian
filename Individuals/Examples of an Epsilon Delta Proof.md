**Tags:** #Collection #Analysis/Proofs #Course/FPM 

![[Epsilon Delta Function Limits#^e6f084]]

> [!Example]+ [[Examples of an Epsilon Delta Proof|Example 1: ]] Let $f(x)=5x+2$. Prove $\displaystyle\lim_{x \to 3}f(x)=17$
> Let $\epsilon>0$. We are assuming that $\lvert x-3 \rvert < \delta$ for whatever $\delta$ we choose. Assume that the conclusion holds,
> $$\lvert f(x)-L \rvert < \epsilon $$
> And then we can substitute to try and unwind this statement to reach the $\delta$ statement above. If we can do this then we can claim that a $\delta$ can be found for every $\epsilon$.
> $$\begin{align}
\lvert f(x)-L \rvert &<\epsilon \\
\lvert 5x+2-(15+2) \rvert &<\epsilon \\
\lvert 5x-15 \rvert &<\epsilon \\
5\cdot\lvert x-3 \rvert &<\epsilon \\
\lvert x-3 \rvert &<\frac{\epsilon}{5} \\
\end{align}
> $$
> From this, we now have a statement that looks the same as $\lvert x-3 \rvert<\delta$. So, therefore we can let $\delta= \displaystyle\frac{\epsilon}{5}$ and then rewrite the above to formally prove that the statement is true.
> 
> **Proof:** Let $\epsilon>0$, and let $\delta=\frac{\epsilon}{5} > 0$. Then for any $x$ where $0<\lvert x-3 \rvert < \delta$,
> $$\begin{align}
\lvert f(x)-L \rvert &= \lvert 5x+2 - (15+2) \rvert \\
&= \lvert 5x-15 \rvert  \\
&= 5\cdot\lvert x-3 \rvert  \\
&<5\cdot\delta \\
&=5\cdot \frac{\epsilon}{5} \\
&= \epsilon
\end{align}
> $$

> [!Example]+ [[Examples of an Epsilon Delta Proof|Example 2: ]] For $f(x)=\displaystyle\frac{3x^{2}-12}{x-2}$, Prove $\displaystyle\lim_{x \to 2}f(x)=12$
> We are trying to reach $\lvert x-2 \rvert<\delta$. Same as above, substitute and unwind the statement
> $$\begin{align}
\lvert f(x)-L \rvert &< \epsilon \\
\left\lvert  \displaystyle \frac{3x^{2}-12}{x-2}-12 \right\rvert  & < \epsilon \\
\left\lvert  \frac{3(x-2)(x+2)}{x-2} \right\rvert  & <\epsilon \\
\lvert 3(x+2) - 12\rvert  & <\epsilon \\
3\cdot\lvert (x+2)-4 \rvert &<\epsilon \\
 3\cdot\lvert x-2 \rvert & <\epsilon \\
\lvert x-2 \rvert < \frac{\epsilon}{3} \\
\end{align}
> $$
> Therefore since we have reached $\lvert x-2 \rvert$, we can let $\delta= \frac{\epsilon}{3}$.
> 
> **Proof:** Let $\epsilon>0$, and let $\delta= \frac{\epsilon}{3}>0$. Then for any $x$ where $0<\lvert x-2 \rvert<\delta$,
> $$\begin{align}
\lvert f(x)-L \rvert &= \left\lvert  \frac{3x^{2}-12}{x-2}-12  \right\rvert  \\
&=\left\lvert  \frac{3(x-2)(x+2)}{x-2}-12 \right\rvert  \\
&= \lvert 3(x+2)-12 \rvert \\
&=3\cdot\lvert (x+2)-4 \rvert \\
&=3\cdot \lvert x-2 \rvert \\
&<3\cdot\delta \\
&=3\cdot \frac{\epsilon}{3} \\
&=\epsilon
\end{align}
> $$

> [!Example]+ [[Examples of an Epsilon Delta Proof|Example 3:]] For $f(x)=x^{2}$, Prove $\displaystyle\lim_{x \to 2}f(x)=4$
> We are trying to reach $\lvert x-2 \rvert < \delta$. Substitute and unwind:
> $$\begin{align}
\lvert f(x)-L \rvert &< \epsilon \\
\lvert x^{2}-4 \rvert &< \epsilon \\
\lvert x+2 \rvert \lvert x-2 \rvert &< \epsilon
\end{align}
> $$
> Now, we need an upper bound for $\lvert x+2 \rvert$ to know how small to choose $\delta$. Since we are discussing the limit as $x$ approaches $2$, we can use a process similar to choosing a fittingly large $n$ to show a sequence will eventually converge to a certain point. If we agree that our $\delta$ neighbourhood (denoted by $V_{\delta}(c)$) around $c=2$ must have radius no bigger than $\delta=1$, then we can get an upper bound of
> $$\lvert x+2 \rvert \le \lvert 3+2 \rvert =5\text{, for all } x \in V_{\delta}(c)$$
> From this, it follows that
> $$\begin{align}
5\cdot\lvert x-2 \rvert &<\epsilon \\
\lvert x-2 \rvert &< \frac{\epsilon}{5}
\end{align}
> $$
> and we can choose $\delta=\min{\{1, \epsilon/5}\}$. A formal proof can then be written like the examples above.

