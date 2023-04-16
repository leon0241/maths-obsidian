#### Poly time tree algorithm
```
(1) get level of each node
(2) initialise empty kv0 array
(3) initialise empty kv1 array

(4) for each level (going from max -> 0):
(5)		for each node on that level:
(6)			calculate kv0 using child nodes
(7)			calculate kv1 using child nodes

(8) set IS to max(kv0 of root, kv1 of root)
(9) return IS
```
- Line 1 is $O(n)$ (goes through all nodes $n$)
- Line 4 is $O(n)$ (worst case $n$ connected nodes all in a line)
- Line 5 is $O(n)$ (worst case $n - 1$ connected nodes to the root)
- Line 6,7 is $O(1)$ (worst case is do $1$ operation i.e. lookup on kv1/kv0 array)
- Line 8 is $O(1)$

![[Pasted image 20230328193341.png]]


Therefore lines 4 through 7 is $O(n)$
Therefore the total time complexity of the algorithm is $O(n)$

