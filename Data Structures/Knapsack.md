
We have a table of items that have weight and monetary value attributes

How can we fill a knapsack with capacity W with the most valuable items

# Using Generate and Test
```Python
maxValue = -1;
maxSubset = {};
for subset in table { # Since we're looping over subsets we loop 2^n times
	if (sum(subset.weight) > W) continue;
	if (sum(subset.value) > maxValue) {
		maxSubset = subset;
	}
}
return maxSubset;
```

Time complexity of $\large O(n2^{n})$

