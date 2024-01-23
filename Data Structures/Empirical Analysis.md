### Basic Operation

The operation in the algorithm that we are choosing to look at in the analysis


### Worst Case

### Best Case

### Average Case


### Example - Sequential Search

```Python
seq_search(A, k)
	i = 0
	while (i < n && A[i] != k)
		i = i + 1
	if (i < n) return i
	return -1
```
##### Best Case:
k is the first item
$\large C(n) = 1$

##### Worst Case:
k is not in A
$\large C(n) = \sum\limits_{i=0}^{n-1}1 = n$

##### Average Case:
We will assume
1. No duplicates
2. Evenly distributed keys (uniformly at random)

We can generalize an average case by looking at probabilities that k is in A
$\large p\in[0,1]$

$\Large C_{AVG}(n) = pC_{in}(n) + (1-p)C_{out}(n)$

Where $\Large C_{in} = \frac{1}{n}\sum\limits_{i=1}^{n} i = \frac{n+1}{2}$
so 

$\Large C_{AVG}(n) = p \frac{n+1}{2}+(1-p)n = $
