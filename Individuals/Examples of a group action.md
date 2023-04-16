**Tags:** #Collection #Algebra/Groups #Course/FPM 

> [!Example]+ [[Examples of a group action|Example: ]] Left Action
>**Definition:** Let $(G,*)$ be a group and $X=G$. For $g$ in $G$ and $x$ in $X$, define
> $$g\cdot x = g * x$$
> For all $x$ in $X$,
> $$e\cdot x = e*x = x$$
> For all $g,h$ in $G$ and all $x$ in $X$,
> $$g\cdot(h\cdot x)=g*(h*x)=(g*h)*x=(g*h)\cdot x$$
> Therefore $g\cdot x=g*x$ is an action of $G$ on itself.
> **Orbit:** The orbit of $x$ is
> $$\text{Orb}(x)=\{g\cdot x\,|\,g\in G\} = \{g*x\,|\, g\in G\} = G$$
> **Stabilizer:** The stabilizer of $x$ is
> $$\text{Stab}(x) = \{g\in G\,|\,g\cdot x=x\} = \{g\in G\,|\,g*x=x\} = \{e\}$$

> [!Example]+ [[Examples of a group action|Example: ]] Right Action
> Let $(G,*)$ be a group and $X=G$. For $g\in G$ and $x \in X$, define
> $$g\cdot x=x*g^{-1}$$
> For all $x \in X$,
> $$e\cdot x=x*e^{-1}=x*e=x$$
> For all $g,h\in G$ and all $x \in X$,
> $$\begin{align}
g\cdot (h\cdot x) &= g\cdot (x*h^{-1}) = (x*h^{-1})*g^{-1} \\
&= x*(h^{-1}*g^{-1}) = x*(g*h)^{-1}=(g*h)\cdot x
\end{align}
> $$
> Therefore, $g\cdot x=x*g^{-1}$ is an action of $G$ on itself.

> [!Example]+ [[Examples of a group action|Example: ]] Conjugate Action
> **Definition:** Let $(G,*)$ be a group and $X=G$. For $g\in G$ and $x \in X$, define
> $$g\cdot x = g*x*g^{-1}$$
> For all $x \in X$,
> $$e\cdot x = e*x*e^{-1}=x$$
> For all $g,h\in G$ and all $x \in X$,
> $$\begin{align}
g\cdot(h\cdot x) &= g\cdot (h*x*h^{-1})=g*(h*x*h^{-1})*g^{-1} \\
&=(g*h)*x*(g*h)^{-1}=(g*h)\cdot x
\end{align}
> $$
> Therefore $g\cdot x=g*x*g^{-1}$ is an action of $G on itself.
> **Orbit:** The orbit of an element $x \in X = G$ is 
> $$\text{Orb}(x)=\{g\cdot x\,|\, g\in G\}=\{gxg^{-1}\,|\,g\in G\}$$
> This set is known as the *conjugacy class* of $x$.
> **Stabilizer:** The stabilizer of $x \in X=G$ is
> $$\begin{align}
\text{Stab}(x)&=\{g\in G\,|\,g\cdot x=x\}=\{g\in G\,|\,gxg^{-1}=x\} \\
&=\{g\in G\,|\,gx=xg\} = C(x)
\end{align}
> $$
> This is known as the *centralizer* of $x$. It is a subgroup of $G$.

