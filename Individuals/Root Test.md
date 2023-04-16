**Tags:** #Theorem #Analysis/Series #Course/FPM 

>[!Theorem]+ Thm: [[Root Test]]
>Let $\dsumzinf a_n$ be a series with non-negative terms such that
>$$\sqrt[n]{a_n} \to L$$
> where $0 \le L \le +\infty$.
> - If $0\le L < 1$ then the series $\dsumzinf a_n$ converges.
> - If $L > 1$ then the series $\dsumzinf a_n$ diverges.
> - If $L = 1$, the series may or may not converge

^ac4c65

###### Logic
If $a_n\ge 0$ for all n, and $\sqrt[n]{a_n} \to L < 1$, then, for every $\epsilon$,
$$\sqrt[n]{a_n} < L + \epsilon \text{, eventually}$$
Choose $\epsilon$ so that $L + \epsilon < 1$. Then
$$a_n < (L + \epsilon)^n = r^n \text{ eventually,}$$where $r = L + \epsilon < 1$. Therefore $\dsumzinf a_n$ converges.
%%EOF%%