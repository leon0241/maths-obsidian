**Tags:** #Theorem #Algebra/Groups #Course/FPM 

> [!Theorem]+ Thm: [[Coprime Cyclic Theorem]]
> Let $m,n\in \N$, let $G=\langle g \rangle$ be a [[Cyclic Subgroups|cyclic group]] of [[Order of a Group#Order of a Group|order]] $m$ and $H=\langle h \rangle$ be a cyclic group of order $n$. Then
> $$G \times H \text{ is cyclic} \iff m \text{ and } n \text{ are coprime (i.e. gcd(m,n) = 1)}$$

#### Example
$\Z_{2} \times \Z_{3}=\{0,1\}\times \{0,1,2\} = \{(0,0), (0,1), (0,2), (1,0), (1,1), (1,2)\}$
If we take a generator of $\{1,1\}$ then $\langle \{1,1\} \rangle$ will cycle through all elements
$$\begin{align}
e &= \{1,1\} \qquad \{1,1\}^1=\{1,1\}\\
\{1,1\}^2&=\{0,2\} \qquad \{1,1\}^3=\{1,0\}\\
\{1,1\}^4&=\{0,1\} \qquad \{1,1\}^5=\{1,2\} \\
\{1,1\}^6&=\{0,0\} \qquad \{1,1\}^7= \{1,1\} = e
\end{align}
$$
