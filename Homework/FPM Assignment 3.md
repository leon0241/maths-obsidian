**Tags:** #Course/FPM #Homework

> [!question] 
> A subgroup $N$ is of a group $G$ is said to be *normal* iff every left coset of $N$ is equal to the corresponding right coset, i.e.
> $$\forall k \in G \quad kN=Nk$$
> Find all subgroups of the dihedral group $D_{3}$. For each subgroup, determine whether it is normal or not.

The elements in $D_{3}$ are $\{e, g, g^{2}, h, hg, hg^{2}\}$  where $g$ is a rotation of $\frac{2\pi}{3}$, and $h$ is a reflection
There are limits to what will count as a valid subgroup:
**Closure**
- $g*h=gh\implies$If $g, h$ are in a subgroup, then so is $hg$.
- $h*hg=e*g=g\implies$ If $h,hg$ are in a subgroup, then so is $g$.
- $g^{2}*h=g^{2}h\implies$ If $g^{2}, h$ are in a subgroup, then so is $hg^{2}$.
- $h*hg^{2}=e*g^{2}=g^{2}\implies$ If $h,hg^{2}$ are in a subgroup, then so is $g$.

**Inverse**
- The inverse of $g$ is $g^{2} \implies$ if $g$ is in a subgroup, so is $g^{2}$
- The inverse of $g^{2}$ is $g \implies$ if $g^{2}$ is in a subgroup, so is $g$
- The inverse of $h, hg, hg^{2}$ is $h, hg, hg^{2}$ respectively.
Therefore, from these restrictions, there are six valid subgroups.
$$\{1\},\,\{1,\,h\},\,\{1,\,hg\},\,\{1,\,hg^{2}\},\,\{1,\,g,\,g^{2}\}, \, \{1,\, g,\, g^{2},\, h,\, hg,\, hg^{2}\}$$

**Showing what subgroups are normal**
A subgroup $N$ is normal if for every $k$ in a group $G$, the left coset $kN$ is equal to the right coset $nK$
1. The subgroup $\{1\}$ is normal trivially, as $e*g=g*e\quad\forall g\in G$
2. The subgroup $\{1,\,h\}$
3. The subgroup $\{1,\,hg\}$
4. The subgroup $\{1,\,hg^{2}\}$
5. The subgroup $\{1,\,g,\,g^{2}\}$ is normal
6. The subgroup $\{1,\, g,\, g^{2},\, h,\, hg,\, hg^{2}\}$ is normal, as "$\forall k\in G$"

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
**Case 1**: If $a<1$, then as $n\to\infty$, $a^n$ is decreasing. Therefore $a^n\to 0$ as $n\to \infty$.
As $n \to \infty$, the $\displaystyle\binom{n}{k}\frac{2^ka^{n-k}}{n^k}$ and $\displaystyle\binom{n}{k}\frac{1}{n^k}$ terms will approach 0, effectively cancelling them out.
$$\frac{\displaystyle a^n +\binom{n}{1}\frac{2a^{n-1}}{n} + \binom{n}{2}\frac{2^2a^{n-2}}{n^2} + \cdots+\binom{n}{n-1}\frac{2^{n-1}a}{n^{n-1}}  + \frac{2^n}{n^n}} {\displaystyle 1+\binom{n}{1} \frac{1}{n}+\binom{n}{2} \frac{1}{n^2}+\cdots+\binom{n}{n-1} \frac{1}{n^{n-1}} + \frac{1}{n^n}} \implies \frac{a^n}{1}=a^n=L_{1}$$
Since $a^n\to 0$ as $n\to\infty$, $L_{1}\to 0$ and via the root test, the series converges via the root test.

**Case 2:** if $a=1$, then as $n\to \infty$, $a^n\to1$.
$$\frac{\displaystyle 1 +\binom{n}{1}\frac{2}{n} + \binom{n}{2}\frac{2^2}{n^2} + \cdots+\binom{n}{n-1}\frac{2^{n-1}}{n^{n-1}}  + \frac{2^n}{n^n}} {\displaystyle 1+\binom{n}{1} \frac{1}{n}+\binom{n}{2} \frac{1}{n^2}+\cdots+\binom{n}{n-1} \frac{1}{n^{n-1}} + \frac{1}{n^n}} = L_{2}$$
From this, you can clearly see that as $2>1,\,2^2>1,\,2^3>1\, \dots$, this means the denominator will be larger than the numerator as $n\to\infty$, therefore $L_{2}>1$, therefore via the root test the series diverges.
**Case 3:** if $a>1$, then as then as $n\to \infty$, $a^n >1$. 
$$\frac{\displaystyle a^n +\binom{n}{1}\frac{2a^{n-1}}{n} + \binom{n}{2}\frac{2^2a^{n-2}}{n^2} + \cdots+\binom{n}{n-1}\frac{2^{n-1}a}{n^{n-1}}  + \frac{2^n}{n^n}} {\displaystyle 1+\binom{n}{1} \frac{1}{n}+\binom{n}{2} \frac{1}{n^2}+\cdots+\binom{n}{n-1} \frac{1}{n^{n-1}} + \frac{1}{n^n}} = L_{3}$$
Since $L_{3} \ge L_{2}$ for all $n$, then by the comparison test since $L_{2}$ diverges, so must $L_{3}$

Therefore, from these three results we can see that for the series
$$\displaystyle\sum_{n=1}^{\infty} \left( \frac{an+2}{n+1} \right)^{n^{2}}$$
The series will converge if $a<0$, and it will diverge if $a\ge 0$.