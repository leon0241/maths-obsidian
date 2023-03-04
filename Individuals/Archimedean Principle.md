**Tags:** #Analysis/Reals  #Theorem #Course/FPM 

> [!Theorem]+ [[Archimedean Principle]]
> Given positive real numbers $a,b\in\R$ there is an integer $n\in\N$ such that $b<na$

^7feff5

#### Idea
Shows that even if $a$ is quite small, and $b$ is quite large then some integer multiple of $a$ will exceed $b$. This is like saying a bathtub can be emptied with a spoon given enough time.

#### Proof
If $b<a$ then we set $n=1$ and it is trivially true.
Otherwise, denote the set $E$ as the set $\{ k\in\mathbb{N}: ka\le b \}$. $E$ is nonempty since $1\in E$. $E$ is also bounded because $ka\le b \iff k\le \frac{b}{a}$, therefore $\frac{b}{a}$ is an upper bound of $E$. Then, by the completeness axiom $s = sup(E)$ exists. Also from [[Axiom of Completeness#Inclusion of Natural Suprema|Inclusion of Natural Suprema]], since $E\in\N$, then $s\in E$. Set $n=s +1$ and therefore $n\in\N$ and $na>b$ so the claim holds.
