#2-6 
Finding the worst case big O of an algorithm

### Alg. Sequential Search 
- Params: List L, item x
- n = length of L
```Java
int i = 1;
while (x != L[i] && i<n) {
	i++;
}
if (L[i] == x)
	print("FOUND")
else
	print("NOT_FOUND")
```

- Worst case is $O(n)$
- Best case is $O(1)$

```Java
// Recursive Version
Search(List L, item x, int i, int n) {
	if ( i > n) {
		print("NOT_FOUND")
	} else {
		if (L[i] == x)
			print("FOUND")
		else
			Search(L, x, i+1, n)
	}
}
```