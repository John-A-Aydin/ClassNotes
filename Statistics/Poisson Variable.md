$\Large X$      $\Large 1, 2, 3, ...$

$\Large P(X=x) = \frac{e^{-\lambda}\lambda^x}{x!}$

$\large \lambda = \mu =$ mean

$\large N =$ span  

### In R
```R
#P(X = x)
dpois(x, lambda*N)

#P(X <= x)
ppois(x, lambda*N)

#Generates random values of n
rpois(n, lambda)
```
