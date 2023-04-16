**Tags:** #Theorem #Analysis/Series #Course/FPM 

> [!Theorem]+ Thm: [[Cauchy's Condensation Test]]
> Let $(a_n)_{n\in\N}$ be a [[Monotone Sequences|decreasing sequence]]  with non-negative terms. Then the following are equivalent:
> 1. The series $\dsumoinf a_n$ converges 
> 2. The series $\dsumzinf 2^na_{2^n}$ converges.

^51fa82

###### Proof

^a8f3be

For $n\in\N$ define
- $S_n = a_1 + a_2 + a_3 + \cdots + a_n$,
- $T_n = A_1 + 2a_2 + 4a_4 + 8a_8 + \cdots + 2^{n-1}a_{2^{n-1}}$

Group the terms in $S_{2^n}$ like
$$S_{2^n} = a_1 + a_2 + (a_3 + a_4) + (a_5 + a_6+a_7+a_8)+\cdots+(a_{2^{n-1}+1} +a_{2^{n-1}+2} +\cdots+a_{2^n})$$
Since $a_n$ has to be decreasing, $(a_3+a_4) > 2a_4$ and the same follows for the rest
$$
\begin{align}
S_{2^n} &= \ccolO a_1 \ccolD+ \ccolB a_2 \ccolD+ \ccolR (a_3 + a_4) \ccolD +\ccolG(a_5 + a_6+a_7+a_8) \ccolD+\cdots+ \ccolY (a_{2^{n-1}+1} +a_{2^{n-1}+2} +\cdots+a_{2^n})\\
&\ge \ccolO a_1 \ccolD + \ccolB a_2 \ccolD + \ccolR 2a_4 \ccolD + \ccolG 4a_8 \ccolD +\cdots+ \ccolY 2^{n-1}a_{2^n} \\
&=\ccolD\frac{1}{2}\ccolO a_1 + \ccolD\frac{1}{2}(\ccolO a_1 \ccolD+\ccolB 2a_2 \ccolD+\ccolR 4a_4 \ccolD+ \ccolG8a_8 \ccolD+\cdots+ \ccolY 2^na_{2^n}) \\
&=\ccolD\frac{1}{2}\ccolO a_1 + \ccolD\frac{1}{2}(\ccolO a_1 \ccolD+\ccolB 2a_2 \ccolD+\ccolR 4a_4 \ccolD+ \ccolG8a_8 \ccolD+\cdots+ \ccolY 2^na_{2^n}) \\
&=\frac{1}{2}\ccolO a_1 \ccolD + \frac{1}{2}T_{n+1} \quad\implies\quad T_{n+1} \le 2(S_{2^n} - \frac{\ccolO a_1}{\ccolD 2})
\end{align}
$$
Similarly,
$$
\begin{align}
S_{2^n} &= \ccolO a_1 \ccolD+ \ccolB a_2 \ccolD+ \ccolR (a_3 + a_4) \ccolD +\ccolG(a_5 + a_6+a_7+a_8) \ccolD+\cdots+ \ccolY (a_{2^{n-1}+1} +a_{2^{n-1}+2} +\cdots+a_{2^n})\\
 &\le \ccolO a_1 \ccolD + \ccolB a_2 \ccolD + \ccolR 2a_2 \ccolD + \ccolG 4a_4 \ccolD +\cdots+ \ccolY 2^{n-1}a_{2^{n-1}} \\
&= a_2 + T_n
\end{align}
$$
Using these two conclusions,
- If $\dsumoinf a_n$ converges, then $(S_n)_{n\in\N}$ is bounded. By (1), $(T_n)_{n\in\N}$ is bounded, therefore $\dsumzinf 2^na_n$ converges.
- If $\dsumzinf 2^na_n$ converges, then $(T_n)_{n\in\N}$ is bounded. By (2), $(S_{2^n})_{n\in\N}$ is bounded, therefore $(S_n)_{n\in\N}$ is bounded (because $S_n \le S_{2^n}$), therefore $\dsumoinf a_n$ converges.
#### Examples

> [!example] Ex: [[Cauchy's Condensation Test|P-series test verification]]
> The series $\dsumoinf \dfrac{1}{n^p}$ converges iff $p > 1$.
> - Assume that $p > 0$. Then, $\dfrac{1}{n^p}$ is decreasing. By Cauchy's Condensation Test, the series $\dsumoinf \dfrac{1}{n^p}$ converges iff the series $\dsumzinf 2^n\dfrac{1}{(2^n)^p}$ converges. Observe that
$$2^n\dfrac{1}{(2^n)^p} = 2^{-np+n} = 2^{-(p-1)n} = \Big( \dfrac{1}{2^{p-1}}\Big)^n$$
  The geometric series $\dsumzinf \bigg(\dfrac{1}{2^{p-1}}\bigg)^n$ converges iff $\dfrac{1}{2^{p-1}} < 1$ ([[Geometric Series Test#^691af3|geometric series test]]), which is equivalent to $p>1$.
> - If $p\le0$, then $\dfrac{1}{n^p} = n^{-p} \not\to 0$, therefore the series $\dsumoinf \dfrac{1}{n^p}$ diverges.

^fd4b54


%%EOF%%