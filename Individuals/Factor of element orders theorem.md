**Tags:** #Theorem #Algebra/Groups #Course/FPM #TODO 

> [!Theorem]+ Thm: [[Factor of element orders theorem]]
> Let $G$ be a finite group and let $a\in G$. Then
> - the order of $a$ is a factor of $\lvert G \rvert$.
> - $a^{\lvert G \rvert}=e$

#### Proof
Let the order of $a$ be $k$
- The cyclic subgroup $\langle a \rangle$ of $G$ has order $k$. By Lagrange's Theorem, $k$ is a factor of $\lvert G \rvert$.
- By the first statement, $k$ divides $n$, so $n=kq$ for some $q$. Since $k$ is a factor of $\lvert G \rvert$, this means that $a^{\lvert G \rvert}=e^q = e$
