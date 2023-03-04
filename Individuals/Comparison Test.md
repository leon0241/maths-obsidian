**Tags:** #Theorem #Analysis/Series #Course/FPM

>[!Theorem]+ Thm: [[Comparison Test]]
> Let $(a_n)_{n\in\N}$ and $(b_n)_{n\in\N}$ be two sequences such that $0\leq a_n\leq b_n$ for all n.
> 1. If $\sum_n b_n$ converges, then $\sum_n a_n$ converges as well.
> 2. If $\sum_n a_n$ diverges, then $\sum_n b_n$ diverges as well.

^c38bd1

###### Proof
We prove the first part (the second part is the contrapositive of the first part).
Since $a_n\leq b_n$ for all $n$, it follows that 
$$0\leq a_1 + a_2 + \cdots+a_n \le b_1 + b_2 + \cdots + b_n$$
If $\sum_n b_n$ converges, then $b_1 + b_2 + \cdots + b_n$ is bounded, therefore $a_1 + a_2 + \cdots + a_n$ is bounded as well, therefore $\sum_n a_n$ converges