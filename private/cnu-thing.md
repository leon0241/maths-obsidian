- $10^k$ has $k+1$ number of digits. e.g. $10^2$ has $3$ digits
- The square root of an even power of $10$ can be written as
$$10^{k} =10^{2n}=10^{2\cdot n} = (10^n)^2$$
therefore $\sqrt{10^{2n}} = 10^n$ i.e. $10^k$ has $\frac{k}{2}+1$ digits
- The square root of $10$ to a power of $k-1$ (rewrite odd as an even number minus $1$) can be thought of as bounded between two even powers of $10$
$$10^{k-1}\in(10^{k-2},10^{k})$$
therefore $\sqrt{10^{k-1}}$ can be thought of as
$$\begin{align}
\sqrt{10^{k-1}} &\in(\sqrt{10^{k-2}},\sqrt{10^{k}}) \\
&\in \left(10^{k/2-1}, 10^{k/2}\right) \\
&\in \left( \frac{k}{2} \text{ digit element}, \frac{k}{2}+1 \text{ digit element}\right)
\end{align}
$$
Therefore, $\sqrt{10^{k-1}}$ has $\frac{k}{2}$ digits, since it is bounded by the first $\frac{k}{2}+1$ digit element. i.e. $10^{k-1}$ has $\frac{k}{2}$ digits.

For any number $n$, it will be bounded by two powers of $10$. For example, a $5$ digit number is bounded between $10,000$ and $100,100$. More formally,
$$\text{For some }n\in \mathbb{N} \text{ with } k\text{ digits}, \quad n\in[10^{k-1}, 10^{k})$$
- The square root of $n$ will also be bounded. If $k$ is even, then it is bounded by 
$$\begin{align}
n&\in (\text{odd power of 10}, \text{even power of 10}) \\
&\in \left(\frac{k}{2} \text{ digit number}, \frac{k}{2}+1 \text{ digit number} \right) \\
&\implies n \text{ is a }\frac{k}{2} \text{ digit number}
\end{align}
$$
- while if $k$ is odd, then it is bounded by
$$\begin{align}
n&\in(\text{even power of 10}, \text{odd power of 10}) \\
&\in\left( \frac{k-1}{2}+1 \text{ digit number}, \frac{k+1}{2} \text{ digit number}\right) \\
&\implies n\text{ is a }\frac{k+1}{2} \text{ digit number}
\end{align}
$$