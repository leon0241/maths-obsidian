**Tags:** #Algebra/Groups #Notation #Course/FPM 
###### [[Subgroup notation|Notation of dropping operators]]
> [!Notation]+
> When dealing with a general group $G$, as much as possible we will write $gh$ for $g*h$

###### Reasoning
Just to make life easier, but when dealing with groups under addition it may be confusing as we are used to $*$ for multiplication.

###### [[Subgroup notation|Notation of power operators]]
> [!Notation]+
> It is useful to have a shorthand for expression such as $g*\dots*g$. If $G$ is a group, $g\in G$ and $k\in\Z$, we define the power $g^k$ by
> $$g^k := \begin{cases}
\hspace{12pt}\overbrace{g*\dots*g}^{k} &\text{if } k>0 \\
\hspace{30pt} e &\text{if } k = 0 \\
\underbrace{ g^{-1}*\dots*g^{-1} }_{ -k } &\text{if } k < 0
\end{cases}
> $$