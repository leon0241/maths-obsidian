**Tags:** #Course/FPM #Homework

## Question 1
> [!question] 
> A subgroup $N$ is of a group $G$ is said to be *normal* iff every left coset of $N$ is equal to the corresponding right coset, i.e.
> $$\forall k \in G \quad kN=Nk$$
> Find all subgroups of the dihedral group $D_{3}$. For each subgroup, determine whether it is normal or not.

The elements in $D_{3}$ are $\{e, g, g^{2}, h, hg, hg^{2}\}$  where $g$ is a rotation of $\frac{2\pi}{3}$, and $h$ is a reflection
There are limits to what will count as a valid subgroup:
Below is a table of each possible operation in $D_{3}$, where going down is the first element, and going along is the second element. e.g. $g*h=hg^2$

| $\large *$    | $\large 1$        | $\large g$    | $\large g^2$  | $\large h$    | $\large hg$   | $\large hg^2$ |
| ------ | ---------- | ------ | ------ | ------ | ------ | ------ |
| $\large 1$    | $\ccolL 1$ | $\ccolL g$    | $\ccolL g^2$  | $\ccolL h$    | $\ccolL hg$   | $\ccolL hg^2$ |
| $\large g$    | $\ccolL g$        | $\ccolL g^2$  | $\ccolL 1$    | $\ccolL hg^2$ | $\ccolL h$    | $\ccolL hg$   |
| $\large g^2$  | $\ccolL g^2$      | $\ccolL 1$    | $\ccolL g$    | $\ccolL hg$   | $\ccolL hg^2$ | $\ccolL h$    |
| $\large h$    | $\ccolL h$        | $\ccolL hg$   | $\ccolL hg^2$ | $\ccolL 1$    | $\ccolL g$    | $\ccolL g^2$  |
| $\large hg$   | $\ccolL hg$       | $\ccolL hg^2$ | $\ccolL h$    | $\ccolL g^2$  | $\ccolL 1$    | $\ccolL g$    |
| $\large hg^2$ | $\ccolL hg^2$     | $\ccolL h$    | $\ccolL hg$   | $\ccolL g$    | $\ccolL g^2$  | $\ccolL 1$    |

**Inverse**
- From the table, there are 6 operations between elements that have an inverse. Those are, $1*1, \,g*g^2,\,g^2*g,\,h*h,\,hg*hg,\,hg^2*hg^2$. Therefore, any subgroup that has elements that aren't included in these 6 are invalid.
- Additionally, the inverse of $g$ being $g^2$ implies that if a group includes $g$, it must also include $g^2$. From this we can prove that there are no 5 element groups. 

**Closure**
- For a 2 element subgroup $\{1,a\}$, any group that includes the identity passes under closure, in this case: $\{1\},\,\{1,\,g\},\,\{1,\,g^{2}\},\,\{1,\,h\},\,\{1,\,hg\},\,\{1,\,hg^2\}$. However, since $g$ and $g^2$ have to be in a set together, this excludes $\{1,g\}, \{1,g^2\}$
- For a 3 element subgroup $\{1,a,b\}$, if $a*b$ returns the identity, then it passes under closure (if it returns one of the elements, then the other element is the identity itself), in this case there is 1: $\{1,\, g,\, g^2\}$
- For a 4 element subgroup $\{1,a,b,c\}$, there are no examples. This would require two elements under commutative operation (e.g. $a*b$ and $b*a$) to either return the identity, or return $c$. From the table, for any $a$ and $b$ where $a,b\ne 1$, we can see that either $a*b \ne b*a$, or $a*b=b*a=1$. Therefore, there are no valid 4 element subgroups under closure
- For a 5 element subgroup $\{1,a,b,c,d\}$, there are no examples. A 5 element group can be achieved by taking two elements $a,b$ where $a*b\ne 0$. We have shown in the 4 element case that $a*b\ne b*a$, therefore the 5 elements of the set can be expressed as $\{1,\,a,\,b,\, a*b,\,b*a\}$
	- The first case is if $a$ is $g$ or $g^2$. Since $g*g^2=1$, $b$ cannot be $g^2$ if $a$ is $g$ since the group would therefore have 3 elements. The rest of the elements include a reflection therefore there is no way to achieve $g^2$ from operations $g*b$. However, the inverse of $g$ is $g^2$, therefore if $g^2$ is not achievable as an output, a 5 element group with $g$ fails under closure or inverses. A similar process can be used to prove $g^2$.
	- The second case is if $a,b\not\in \{g,g^2\}$. Therefore, $a,b\in\{h,hg,hg^2\}$. From the table, we can see that the resulting two elements will be $a*b=g, \,b*a=g^2$, or the other way round. Since $a,b$ can only include 2 of the elements in $\{h,hg,hg^2\}$, the set is valid under closure if the third element cannot be obtained from an operation. However, since $g$ and $g^2$ are rotations, the remaining element can be clearly obtained from one of the two elements.
		1. No $h \implies a,b =hg,hg^2$. However, $hg^2*g=h \implies$ Fails
		2. No $hg \implies a,b=h,hg^2$. However, $h*g=hg\implies$ Fails
		3. No $hg^2 \implies a,b=h,hg$. However, $hg*g=hg^2\implies$ Fails
	- Therefore, from this we can conclude there are no 5 element sets in $D_{3}$.
- For a 6 element subgroup, $D_{3}$ is a group, therefore it trivially is a subgroup

Therefore, from these restrictions, there are six valid subgroups.
$$\{1\},\,\{1,\,h\},\,\{1,\,hg\},\,\{1,\,hg^{2}\},\,\{1,\,g,\,g^{2}\}, \, \{1,\, g,\, g^{2},\, h,\, hg,\, hg^{2}\}$$

**Showing what subgroups are normal**

A subgroup $N$ is normal if for every $k$ in a group $G$, the left coset $kN$ is equal to the right coset $nK$

On the lookup table, the cosets of a subgroup $N$ can be visualised as a strip corresponding each element in the set $G$. For example, for the subgroup $\{1,h\}$ can be visualised like so: 
```start-multi-column  
ID: Table1  
number of columns: 2  
```
Left Cosets of $\{1,h\}$

| $\large *$    | $\large 1$        | $\large g$    | $\large g^2$  | $\large h$    | $\large hg$   | $\large hg^2$ |
| ------ | ------ | ------ | ------ | ------ | ------ | ------ |
| $\large 1$    | $\ccolB 1$    | $\ccolL g$    | $\ccolL g^2$  | $\ccolB h$    | $\ccolL hg$   | $\ccolL hg^2$ |
| $\large g$    | $\ccolB g$    | $\ccolL g^2$  | $\ccolL 1$    | $\ccolB hg^2$ | $\ccolL h$    | $\ccolL hg$   |
| $\large g^2$  | $\ccolB g^2$  | $\ccolL 1$    | $\ccolL g$    | $\ccolB hg$   | $\ccolL hg^2$ | $\ccolL h$    |
| $\large h$    | $\ccolB h$    | $\ccolL hg$   | $\ccolL hg^2$ | $\ccolB 1$    | $\ccolL g$    | $\ccolL g^2$  |
| $\large hg$   | $\ccolB hg$   | $\ccolL hg^2$ | $\ccolL h$    | $\ccolB g^2$  | $\ccolL 1$    | $\ccolL g$    |
| $\large hg^2$ | $\ccolB hg^2$ | $\ccolL h$    | $\ccolL hg$   | $\ccolB g$    | $\ccolL g^2$  | $\ccolL 1$    |

--- end-column ---

Right Cosets of $\{1,\,h\}$

| $\large *$    | $\large 1$        | $\large g$    | $\large g^2$  | $\large h$    | $\large hg$   | $\large hg^2$ |
| ------ | ------ | ------ | ------ | ------ | ------ | ------ |
| $\large 1$    | $\ccolG 1$    | $\ccolG g$    | $\ccolG g^2$  | $\ccolG h$    | $\ccolG hg$   | $\ccolG hg^2$ |
| $\large g$    | $\ccolL g$    | $\ccolL g^2$  | $\ccolL 1$    | $\ccolL hg^2$ | $\ccolL h$    | $\ccolL hg$   |
| $\large g^2$  | $\ccolL g^2$  | $\ccolL 1$    | $\ccolL g$    | $\ccolL hg$   | $\ccolL hg^2$ | $\ccolL h$    |
| $\large h$    | $\ccolG h$    | $\ccolG hg$   | $\ccolG hg^2$ | $\ccolG 1$    | $\ccolG g$    | $\ccolG g^2$  |
| $\large hg$   | $\ccolL hg$   | $\ccolL hg^2$ | $\ccolL h$    | $\ccolL g^2$  | $\ccolL 1$    | $\ccolL g$    |
| $\large hg^2$ | $\ccolL hg^2$ | $\ccolL h$    | $\ccolL hg$   | $\ccolL g$    | $\ccolL g^2$  | $\ccolL 1$    |

=== end-multi-column

From the table, we can see that for the elements of $G = \{1,\,g,\,g^2,\,h,\,hg,\,hg^2\}$,
The left cosets of $\{1,h\}$ are
$$\{\{1,\,h\},\,\{g,\,hg^2\},\,\{g^2,\,hg\},\,\{h,\,1\},\,\{hg,\,g^2\},\,\{hg^2,\,g\}\}$$
The right cosets of $\{1,\,h\}$ are
$$\{\{1,\,h\},\,\{g,\,hg\},\,\{g^2,\,hg^2\},\,\{h,\,1\},\,\{hg,\,g\},\,\{hg^2,\,g^2\}\}$$
The left coset is not equal to the right coset in some places, for example $$hgN = \{hg,\,g^2\},\, \quad Nhg=\{hg,\,g\}$$Therefore, the group $\{1,\,h\}$ is not normal.

If we repeat the same process with the group $\{1,\,g,\,g^2\}$, we get:


```start-multi-column  
ID: Table2  
number of columns: 2  
```
Left Cosets of $\{1,g,\,g^2\}$

| $\large *$    | $\large 1$        | $\large g$    | $\large g^2$  | $\large h$    | $\large hg$   | $\large hg^2$ |
| ------ | ------ | ------ | ------ | ------ | ------ | ------ |
| $\large 1$    | $\ccolB 1$    | $\ccolB g$    | $\ccolB g^2$  | $\ccolL h$    | $\ccolL hg$   | $\ccolL hg^2$ |
| $\large g$    | $\ccolB g$    | $\ccolB g^2$  | $\ccolB 1$    | $\ccolL hg^2$ | $\ccolL h$    | $\ccolL hg$   |
| $\large g^2$  | $\ccolB g^2$  | $\ccolB 1$    | $\ccolB g$    | $\ccolL hg$   | $\ccolL hg^2$ | $\ccolL h$    |
| $\large h$    | $\ccolB h$    | $\ccolB hg$   | $\ccolB hg^2$ | $\ccolL 1$    | $\ccolL g$    | $\ccolL g^2$  |
| $\large hg$   | $\ccolB hg$   | $\ccolB hg^2$ | $\ccolB h$    | $\ccolL g^2$  | $\ccolL 1$    | $\ccolL g$    |
| $\large hg^2$ | $\ccolB hg^2$ | $\ccolB h$    | $\ccolB hg$   | $\ccolL g$    | $\ccolL g^2$  | $\ccolL 1$    |

--- end-column ---

Right Cosets of $\{1,\,g,\,g^2\}$

| $\large *$    | $\large 1$        | $\large g$    | $\large g^2$  | $\large h$    | $\large hg$   | $\large hg^2$ |
| ------ | ------ | ------ | ------ | ------ | ------ | ------ |
| $\large 1$    | $\ccolG 1$    | $\ccolG g$    | $\ccolG g^2$  | $\ccolG h$    | $\ccolG hg$   | $\ccolG hg^2$ |
| $\large g$    | $\ccolG g$    | $\ccolG g^2$  | $\ccolG 1$    | $\ccolG hg^2$ | $\ccolG h$    | $\ccolG hg$   |
| $\large g^2$  | $\ccolG g^2$  | $\ccolG 1$    | $\ccolG g$    | $\ccolG hg$   | $\ccolG hg^2$ | $\ccolG h$    |
| $\large h$    | $\ccolL h$    | $\ccolL hg$   | $\ccolL hg^2$ | $\ccolL 1$    | $\ccolL g$    | $\ccolL g^2$  |
| $\large hg$   | $\ccolL hg$   | $\ccolL hg^2$ | $\ccolL h$    | $\ccolL g^2$  | $\ccolL 1$    | $\ccolL g$    |
| $\large hg^2$ | $\ccolL hg^2$ | $\ccolL h$    | $\ccolL hg$   | $\ccolL g$    | $\ccolL g^2$  | $\ccolL 1$    |

=== end-multi-column

The left cosets of the group are:
$$\{\{1,\,g,\,g^2\},\,\{g,\,g^2,\,1\}\{g^2,\,1,\,g\}\{h,\,hg,\,hg^2\},\,\{hg,\,hg^2,\,h\},\,\{hg^2,\,h,\,hg\}\}$$
The right cosets of the group are:
$$\{\{1,\,g,\,g^2\},\,\{g,\,g^2,\,1\},\,\{g^2,\,1,\,g\},\,\{h,\,hg^2,\,hg\},\,\{hg,\,h,\,hg^2\},\,\{hg^2,\,hg,\,h\}\}$$
From this we can see that every left coset is the same as the right coset, therefore the subgroup $\{1,\,g,\,g^2\}$ is normal.

The other subgroups can also be calculated like this but we will just work off counterexamples.
- The subgroup $\{1\}$ is normal trivially, as $e*g=g*e\quad\forall g\in G$
- The subgroup $\{1,\,hg\}$ is not normal, counterexample: $hN=\{h,g\},\,Nh=\{h,\,g^2\}$
- The subgroup $\{1,\,hg^{2}\}$ is not normal, counterample: $hgN=\{hg,\,g\},\,Nhg=\{hg,\,g^2\}$
- The subgroup $\{1,\, g,\, g^{2},\, h,\, hg,\, hg^{2}\}$ is normal. Looking at the graph, the left cosets of the subgroup will effectively be a group of every row in the table, where each row includes every single element of $D_{3}$. The right cosets will be a group of every column in the table, where each column also includes every single element of $D_{3}$. Therefore, all elements of the left and right cosets will be the same, meaning the subgroup $D_{3}$ is normal.

Therefore, the normal subgroups of the dihedral group $D_{3}$ are 
$$\{1\},\, \{1,\,g,\,g^2\},\,\{1,\,g,\,g^2,\,h,\,hg,\,hg^2\}$$

## Question 2
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
Since $a^n\to 0$ as $n\to\infty$, $L_{1}\to 0$ and via the root test, the series converges if $a<1$.

**Case 2:** if $a=1$, then as $n\to \infty$, $a^n\to1$.
$$\frac{\displaystyle 1 +\binom{n}{1}\frac{2}{n} + \binom{n}{2}\frac{2^2}{n^2} + \cdots+\binom{n}{n-1}\frac{2^{n-1}}{n^{n-1}}  + \frac{2^n}{n^n}} {\displaystyle 1+\binom{n}{1} \frac{1}{n}+\binom{n}{2} \frac{1}{n^2}+\cdots+\binom{n}{n-1} \frac{1}{n^{n-1}} + \frac{1}{n^n}} = L_{2}$$
From this, you can clearly see that as $2>1,\,2^2>1,\,2^3>1\, \dots$, this means the denominator will be larger than the numerator as $n\to\infty$, therefore $L_{2}>1$, therefore via the root test the series diverges.
**Case 3:** if $a>1$, then as then as $n\to \infty$, $a^n \to\infty$. 
$$\frac{\displaystyle a^n +\binom{n}{1}\frac{2a^{n-1}}{n} + \binom{n}{2}\frac{2^2a^{n-2}}{n^2} + \cdots+\binom{n}{n-1}\frac{2^{n-1}a}{n^{n-1}}  + \frac{2^n}{n^n}} {\displaystyle 1+\binom{n}{1} \frac{1}{n}+\binom{n}{2} \frac{1}{n^2}+\cdots+\binom{n}{n-1} \frac{1}{n^{n-1}} + \frac{1}{n^n}} = L_{3}$$
Since $L_{3} \ge L_{2}$ for all $n$, then via the comparison test since $L_{2}$ diverges, so must $L_{3}$

Therefore, from these three results we can see that for the series
$$\displaystyle\sum_{n=1}^{\infty} \left( \frac{an+2}{n+1} \right)^{n^{2}}$$
The series will converge if $a<0$, and it will diverge if $a\ge 0$.
%%EOF%%