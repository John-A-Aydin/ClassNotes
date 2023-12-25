
```Python
while (<condition B>)
	P
end while
```

We use Q: loop invariant$$\large \{Q\land B\}P\{Q\land B'\} $$$\large B'$ is the opposite of the loop's conditional
Since the loop ends when the conditional is no longer true, we put the $B'$ in the post condition.
$\large Q$ is the loop's invariant, a condition which is true in every iteration of the program/algorithm at the beginning as well as at the termination of the loop.
$\large P$ is the code that is being executed inside the loop.
### Ex. 

```Python
func(x, y)
	Local variables:
		integer i, j
	i = 0
	j = 0
	while (i != x)
		i = i + 1
		j = j + y
	end while
	
	// j has value x*y
	
	return j
end func
```

We look at it in reverse order:
- Assuming j is equal to y\*x
Conjecture for Q:
	j = i\*y


### Theorem: $\forall k \ge 0 \text{ , }Q_k$
##### Proof by Induction

**Base Case:**
$Q_0$         $j_0= i_0* y_0$
$i_0=0$,   $j_0 = 0$

**Inductive Step:**

$k\ge 0$    $Q_k\rightarrow Q_{k+1}$

$j_{k+1} = \text{}$
1. $j_k+y$
2. $i_k*y+y$
3. $(i_k+1)y$
4. $i_{k+1}*y$
$j_{k+1} = i_{k+1}*y*$



