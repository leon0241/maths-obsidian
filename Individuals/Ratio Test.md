**Tags:** #Theorem #Analysis/Series #Course/FPM

> [!Theorem]+ Thm: [[Ratio Test]]
> Let $\dsumzinf a_n$ be a series with positive terms such that $\dfrac{a_{n+1}}{a_n} \to L$, where $0\le L \le +\infty$.
> - If $0\le L < 1$ then the series $\dsumzinf a_n$ converges.
> - If $L > 1$ then the series $\dsumzinf a_n$ diverges.
> - If $L = 1$:
>   - If $a_n = \dfrac{1}{n}$, then $\dfrac{a_{n+1}}{a_n} = \dfrac{n}{n + 1} \to 1$, and $\dsumzinf \frac{1}{n}$ diverges.>
>   - If $a_n = \dfrac{1}{n^2}$, then $\dfrac{a_{n+1}}{a_n} = \dfrac{n^2}{(n + 1)^2} \to 1$, and $\dsumzinf \frac{1}{n^2}$ converges.

^f43231

###### Logic
If $a_n > 0$ for all n, and $\dfrac{a_{n+1}}{a_n} \to L < 1$, then, for every $\epsilon$,
$$\frac{a_{n+1}}{a_n} < L + \epsilon \text{, eventually.}$$
Choose $\epsilon$ so that $L + \epsilon \in (0, 1)$, and take $N \in\N$ sufficiently large. Then
$$a_n = \frac{a_n}{a_{n-1}}\frac{a_{n-1}}{a_{n-2}}\cdots\frac{a_{N+1}}{a_N} a_n \le (L + \epsilon)^{n - N} a_N = Cr^n$$
where $r = L + \epsilon\in(0,1)$, $C = (L + \epsilon)^{-N}a_N$. Therefore $\dsumzinf a_n$ converges.
%%EOF%%