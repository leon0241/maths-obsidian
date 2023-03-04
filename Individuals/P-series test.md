**Tags:** #Lemma #Analysis/Series #Course/FPM

> [!Lemma]+ Lem: [[P-series test]]
> The series
> $$\dsumoinf \frac{1}{k^p}$$
> converges if and only if p > 1

#### Proof (Cauchy Condensation-like)
Show that the harmonic series $\displaystyle\sum_{n=1}^{\infty} \frac{1}{k}$ diverges
Observe that
$$\begin{align}
 \displaystyle\sum_{n=1}^{\infty} = \frac{1}{k} &= 1 + \frac{1}{2} + \frac{1}{3} + \frac{1}{4} + \frac{1}{5}  +\frac{1}{6} + \frac{1}{7} + \frac{1}{8} + \cdots \\
&= 1+\left( \frac{1}{2} \right)+\left( \frac{1}{3} + \frac{1}{4} \right) + \left( \frac{1}{5} + \frac{1}{6} + \frac{1}{7} + \frac{1}{8}\right) + \cdots \\
&\ge 1 + \left( \frac{1}{2} \right) + \left( \frac{1}{4} + \frac{1}{4} \right) + \left( \frac{1}{8}+\frac{1}{8}+\frac{1}{8}+\frac{1}{8} \right) + \cdots \\
&= 1 + \left( \frac{1}{2} \right) + \left( \frac{1}{2} \right) + \left( \frac{1}{2} \right) + \cdots
\end{align}$$
In particular, if $s_{n}$ is the partial $n^{th}$ partial sum of the harmonic series, then $(s_{n})$ is monotonically increasing and, by the above,
$$s_{2^n} \ge 1 + n\cdot \frac{1}{2}$$
Since $\left( 1+n\cdot \frac{1}{2} \right)$ diverges to $\infty$, by the [[Comparison Test#^c38bd1|comparison test]], the subsequence $s_{2^n}$ also diverges to $\infty$. For a [[Monotone Sequences#^e29b33|monotonically increasing sequence]], if a subsequence diverges to $\infty$ - implying that $(s_{n})$ is unbounded - the entire sequence also diverges to $\infty$ by the [[Monotone Convergence Theorem#^f88f95|monotone convergence theorem]]. This shows that the harmonic series diverges to $\infty$. 

The comparison test can also be used to show that $\displaystyle\sum_{n=1}^{\infty} \frac{1}{k^p},\, p<1$ is divergent. If $p\le 1$, then $\dfrac{1}{k^p} \ge \frac{1}{k}$ for all $k\in\N$. since $\displaystyle\sum_{n=1}^{\infty} \frac{1}{k}$ diverges, then so must $\displaystyle\sum_{n=1}^{\infty} \frac{1}{k^p}$


#### Proof 2 (Cauchy Condensation)
![[Cauchy's Condensation Test#^fd4b54]]