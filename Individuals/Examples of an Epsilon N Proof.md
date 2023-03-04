**Tags:** #Analysis/Proofs #Collection #Course/FPM 
###### [[Examples of an Epsilon N Proof]]
> [!Example]+ Ex: [[Examples of an Epsilon N Proof|Showing 1/n converges to 0]]
> Show that $\frac{1}{n}\to 0$ as $n\to\infty$
> Pick any $\epsilon<0$. From the [[Archimedean Principle]] it follows that there exists $N\in\N$ such that $N>\frac{1}{\epsilon}$ or $\frac{1}{N} < \epsilon$. It follows that if $N\ge N$ then
> $$\left\lvert \frac{1}{n} - 0 \right\rvert = \frac{1}{n}\le \frac{1}{N} < \epsilon $$
> Hence the limit of this sequence is 0

> [!example]+ Ex: [[Examples of an Epsilon N Proof|Showing a complex fraction converges]]
> Show that the sequence $\left( \frac{2n+1}{3n+2} \right)_{n\in\mathbb{N}}$ converges to $\frac{2}{3}$
> We start with the rough work. To show this from the definition we start with an arbitrary $\epsilon>0$ and find an $N_{\epsilon}$ such that $\left\lvert  \frac{2n+1}{3n+2} -\frac{2}{3}  \right\rvert < \epsilon$ for all $n>N_{\epsilon}$. Let's explore this.
> $$\left\lvert  \frac{2n+1}{3n+2}-\frac{2}{3}  \right\rvert =\frac{11}{3(3n+2)} < \epsilon$$
> This inequality is equal to
> $$n> \frac{1}{3}\left( \frac{11}{3\epsilon} -2\right)$$
> *Now write a formal description of said proof:* 
> Let $\epsilon>0$. Pick a positive integer $N$ such that
> $$N>\frac{1}{3}\left( \frac{11}{3\epsilon}-2 \right)$$
> Then,
> $$\frac{11}{3(3N+2)} < \epsilon$$
> For all $n$ with $n\ge N$ we have 
> $$\lvert a_{n}-L \rvert = \left\lvert  \frac{2n+5}{3n+2} - \frac{2}{3}  \right\rvert =\frac{11}{3(3n+2)} \le \frac{11}{3(3N+2)}<\epsilon$$
> another method of finding a limit is,
> $$\left\lvert  \frac{2n+1}{3n+2}-\frac{2}{3}  \right\rvert =\frac{11}{3(3n+2)} = \frac{11}{9n+6} < \frac{11}{9n}< \epsilon$$
> Since $9n+6>9n$, if the left fraction is bounded by the right fraction, and the right fraction is still always smaller than $\epsilon$, then it follows that the left is also smaller than $\epsilon$.
> Therefore, let $\epsilon>0$. Pick a positive integer $N$ such that $N>\frac{11}{9\epsilon}$. Then $\frac{11}{9N} < \epsilon$. For all $n$ with $n\ge N$, we have
> $$\lvert a_{n}-L \rvert = \left\lvert  \frac{2n+5}{3n+2} - \frac{2}{3}  \right\rvert =\frac{11}{9n+6} \le \frac{11}{9n} \le \frac{11}{9N}<\epsilon$$
