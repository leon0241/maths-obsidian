**Tags:** #Algebra/Groups #Theorem #Course/FPM 

> [!Theorem]+ Thm: [[Equivalence Modulo Theorem]]
> Let $G$ be a group, and let $H$ be a subgroup of $G$. Then [[Equivalence Modulo Notation|equivalence modulo]] $H$ is an [[Equivalence Relation|equivalence relation]] on $G$

^6a9f28

###### Proof
By the definition of an [[Equivalence Relation]], we must show that the relation is reflexive, symmetric, and transitive.
- **Reflexive:** if $a \in G$ then $a^{-1}a=e\in H$ and so $a\equiv a \text{ mod } H$.
- **Symmetric:** let $a,b\in G$ be such that $a\equiv b\text{ mod } H$. Then $b^{-1}a\in H$. Now $a^{-1}b=(b^{-1}a)^{-1}\in H$ and so $b\equiv a \text{ mod } H$
- **Transitive:** let $a,b,c\in G$ be such that $a \equiv b \text{ mod } H$ and $b\equiv c\text{ mod } H$. Then, $b^{-1}a\in H$ and $c^{-1}b\in H$, so $c^{-1}a=c^{-1}bb^{-1}a\in H$. Thus $a\equiv c \text{ mod } H$.
