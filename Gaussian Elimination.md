#TODO 

### Implementation for \[n,n+1] matrix
```Python
for i:0..n-2
	for j:i..n-1
		for k:i..n
			A[j,k] = A[j,k] - A[i,k] * A[j,i]/ A[j,i]
```

##### Input size