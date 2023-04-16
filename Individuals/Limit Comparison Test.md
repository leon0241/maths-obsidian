**Tags:** #Theorem #Analysis/Series #Course/FPM

> [!Theorem]+ Thm: [[Limit Comparison Test]]
Let $(a_n)_{n\in\N}$ and $(b_n)_{n\in\N}$ be two real sequences with $a_n\geq0$ and $b_n\geq0$ for all n. Assume that $\dfrac{a_n}{b_n} \to L$ for some $L\in(0,\infty)$. Then, $\dsumoinf a_n$ converges iff $\dsumoinf b_n$ converges.

^f9d4a7

###### Proof
let $\epsilon = L/2$. There exists an index $N$ such that for all indices n with $n\geq N$ we have
$$L-\epsilon\lt\frac{a_n}{b_n}\lt L + \epsilon$$
Therefore: $$\frac{L}{2}<\frac{a_n}{b_n}<\frac{3L}{2}$$
It follows that $$a_n<\frac{3L}{2}b_n$$
for all $n$ with $n\geq N$
By the [[Comparison Test#^c38bd1|comparison test]], if $\dsumoinf b_n$ converges, then $\dsumoinf b_n$ converges as well.
Also, $$b_n < \frac{2}{L}a_n$$
for all $n$ with $n\geq N$.
By the Comparison Test, if $\dsumoinf a_n$ converges then $\dsumoinf b_n$ converges as well
%%EOF%%