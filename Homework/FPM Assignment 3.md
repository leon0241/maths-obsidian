**Tags:** #Course/FPM #Homework
> [!Question]
> Let $a$ be a non-negative real number. Prove that the series
> $$\displaystyle\sum_{n=1}^{\infty} \left( \frac{an+2}{n+1} \right)^{n^{2}}$$
> converges when $a<1$ and diverges when $a\ge 1$.

Via the root test:
$$a_{n} = \left( \frac{an+2}{n+1} \right)^{n^2} \implies \sqrt[n]{a_{n}} =  \sqrt[n]{\left( \frac{an+2}{n+1} \right)^{n^2}} = \left( \frac{an+2}{n+1} \right)^n$$
Therefore, for $\left( \dfrac{an+2}{n+1} \right)^n \to L$, the convergence of the series can be determined.
The fraction can be expanded like so:
$$\left( \frac{an+2}{n+1} \right)^n = \frac{(an+2)^n}{(n+1)^n} = \frac{\overbrace{(an+2)(an+2)\cdots(an+2)}^n{}}{\underbrace{(n+1)(n+1)\cdots(n+1)}_{n}}$$
From the binomial theorem, this can be expanded and divided by $n^n$:
$$\begin{align}
\left( \frac{an+2}{n+1} \right)^n &= \frac{\overbrace{(an+2)(an+2)\cdots(an+2)}^n{}}{\underbrace{(n+1)(n+1)\cdots(n+1)}_{n}} \\&= \frac{\displaystyle a^nn^n + \binom{n}{1}2a^{n-1}n^{n-1} + \binom{n}{2}2^2a^{n-2}n^{n-2} + \cdots+\binom{n}{n-1}2^{n-1}an + 2^n}{\displaystyle n^n+\binom{n}{1}n^{n-1}+\binom{n}{2}n^{n-2}+\cdots+\binom{n}{n-1}n + 1} \\
\\
&=\frac{\displaystyle a^n +\binom{n}{1}\frac{2a^{n-1}}{n} + \binom{n}{2}\frac{2^2a^{n-2}}{n^2} + \cdots+\binom{n}{n-1}\frac{2^{n-1}a}{n^{n-1}}  + \frac{2^n}{n^n}} {\displaystyle 1+\binom{n}{1} \frac{1}{n}+\binom{n}{2} \frac{1}{n^2}+\cdots+\binom{n}{n-1} \frac{1}{n^{n-1}} + \frac{1}{n^n}}
\end{align}$$
**Case 1**: If $a<1$, then $a^n$ as $n\to\infty$ is decreasing. Therefore $a^n\to 0$ as $n\to \infty$.
As $\sqrt[n]{a_{n}} \to \infty$, the $\dfrac{1}{n^x}$ terms will approach 0, effectively cancelling them out.
$$\frac{\displaystyle a^n +\binom{n}{1}\frac{2a^{n-1}}{n} + \binom{n}{2}\frac{2^2a^{n-2}}{n^2} + \cdots+\binom{n}{n-1}\frac{2^{n-1}a}{n^{n-1}}  + \frac{2^n}{n^n}} {\displaystyle 1+\binom{n}{1} \frac{1}{n}+\binom{n}{2} \frac{1}{n^2}+\cdots+\binom{n}{n-1} \frac{1}{n^{n-1}} + \frac{1}{n^n}} \implies \frac{a^n}{1}=a^n=L_{1}$$
Since $a^n\to 0$ as $n\to\infty$, $L_{1}\to 0$ and via the root test, the series converges via the root test.

**Case 2:** if $a=1$, then as $n\to \infty$, $a^n\to1$.
$$\frac{\displaystyle 1 +\binom{n}{1}\frac{2}{n} + \binom{n}{2}\frac{2^2}{n^2} + \cdots+\binom{n}{n-1}\frac{2^{n-1}}{n^{n-1}}  + \frac{2^n}{n^n}} {\displaystyle 1+\binom{n}{1} \frac{1}{n}+\binom{n}{2} \frac{1}{n^2}+\cdots+\binom{n}{n-1} \frac{1}{n^{n-1}} + \frac{1}{n^n}} = L_{2}$$
From this, you can clearly see that as $2>1,\,2^2>1,\,2^3>1\, \dots$, this means the denominator will be larger than the numerator as $n\to\infty$, therefore $L_{2}>1$, therefore the series diverges.
**Case 3:** if $a>1$, then as then as $n\to \infty$, $a^n >1$. 
$$\frac{\displaystyle a^n +\binom{n}{1}\frac{2a^{n-1}}{n} + \binom{n}{2}\frac{2^2a^{n-2}}{n^2} + \cdots+\binom{n}{n-1}\frac{2^{n-1}a}{n^{n-1}}  + \frac{2^n}{n^n}} {\displaystyle 1+\binom{n}{1} \frac{1}{n}+\binom{n}{2} \frac{1}{n^2}+\cdots+\binom{n}{n-1} \frac{1}{n^{n-1}} + \frac{1}{n^n}} = L_{3}$$
Since $L_{3} \ge L_{2}$, then by the comparison test since $L_{2}$ diverges, then so must $L_{3}$

Therefore, from these three results we can see that for the series
$$\displaystyle\sum_{n=1}^{\infty} \left( \frac{an+2}{n+1} \right)^{n^{2}}$$
The series will converge if $a<0$, and it will diverge if $a\ge 0$.