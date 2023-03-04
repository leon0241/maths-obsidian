**Tags:** #Analysis/Proofs #Main #Course/FPM 

> [!Definition]+ Thm: [[Proving a Sequence is Convergent]]
> A sequence of real numbers $(x_{n})$ is said to converge to a real number $L$ if for every $\epsilon>0$ there is $N\in\N$ (where $N$ usually depends on $\epsilon$) such that
> $$\text{for all } n\ge N\quad\text{we have that } \lvert x_{n}-L \rvert <\epsilon $$

![[Convergent Series Notation#^bf97e3]]


###### Idea
The main method to show convergence is to start with an arbitrary $\epsilon$ and find a sufficiently large $N\in\N$. Furthermore, the constraint that $N$ is a natural number is unneccessary. From the [[Archimedean Principle#^7feff5|Archimedean Principle]], we know that for each real number $r$ we can find a natural number $N$ such that $N>r$. With this we can easily swap between the two definitions.

###### [[Examples of an Epsilon N Proof]]