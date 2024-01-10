
### Brute Force for finding powers

Finds $\large a^{p}$ 

```Python
exp(a,p)
	pow = 1 # Start at 1 bc a^0 = 1
	while (p > 0)
		pow *= a
		--p
	return pow
```

Runtime of $\large O(p)$

