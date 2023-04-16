**Tags:** #Definition #Algebra/Categories #Course/Category_Theory 

> [!Definition]+ Def: [[Category of a programming language]]
> Given a functional programming language $L$, there is an associated category where the objects are the data types of $L$, and the arrows are the possible functions of $L$. A basic example of an arrow is shown below in python
> ```python
> def f(a): # Adds 1 to the input
> 	a += 1
> 	return a
> b = f(a)
> ```
> Composition is given by applying another function to the output of $f$, sometimes written as
> $$g\circ f = f;g$$
> The identity function is the "do nothing" program shown above where the input is not modified.

^abc042
