
```Python
exp(a, p)
	if (p = 0) return 1
	else if (p = 1) return a
	else return exp(a, floor(p/2)) * exp(a, ceiling(p/2))
```

Runtime of $\large O(p)$ 
This tree doesn't all go onto the call stack at the same time.
Has an opportunity for [[Data Structures/Dynamic Programming]]
