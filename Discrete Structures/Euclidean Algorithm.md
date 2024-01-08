
Computes the greatest common denominator of a, b (positive integers) recursively

Using what we learned in the [[Correctness of Loops]] we can verify the correctness of this algorithm.

gcd(42, 220) = 2

$42 = 2*3*7$
$220 = 2^2*11*5$

$a = P_1^{\alpha_1}P_2^{\alpha_2}\text{...}P_n^{\alpha_n}$ 
$b = P_1^{\beta_1}P_2^{\beta_2}\text{...}P_n^{\beta_n}$

```Python
gcd(m, n) {
	while n != 0
	r = m % n
	m = n
	n = r
	return m
}
```