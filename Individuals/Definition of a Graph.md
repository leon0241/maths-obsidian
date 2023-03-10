**Tags:** #Algebra/Graphs #Definition #Course/FPM 
###### [[Definition of a Graph]]
> [!Theorem]+
> A graph is a finite set of vertices joined by edges. We will assume that there is at most one edge joining two given vertices and no edge joins a vertex to itself. The valency of a vertex is the number of edges emerging from it.
#### Example

```tikz
\usepackage{tikz-cd}

\begin{document}
	\begin{tikzcd}
	    & 1 \arrow[r,dash] \arrow[d,dash]
	    & 2 \arrow[d, dash] \\
	    & 3 \arrow[r, dash]
	    & 4
	\end{tikzcd}
\end{document}
```