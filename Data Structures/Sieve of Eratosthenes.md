
Takes an integer and returns all primes that are less than or equal to n

```Python
for p in range 2..n
	A[p] = p
for p in range 2..sqrt(n)
	if A[p] != 0 # If the Index is still in the array
		j = p*p # We start at the square of p
		while j <= n # Loop over all multiples of p 
			A[j] = 0 # Destroy them jawns
			j = j + p # Iterate
			
```