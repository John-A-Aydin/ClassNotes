### Finding powers

```Python
exp(a, p)
	if(p = 0) return 1
	else return a*exp(a, p - 1)
```

Runtime of $\large O(p)$
Keep in mind that this linear growth occurs on the stack which is generally worse than other types of growth

```python
exp(a, p)
	if (p = 0) return 1
	else if (p = 1) return a
	else if (p is even)
		temp = exp(a, p/2)
		return temp*temp
	else
		temp = exp(a, floor(p/2))
		return a*temp*temp
```

Runtime of $\large O(log(p))$  