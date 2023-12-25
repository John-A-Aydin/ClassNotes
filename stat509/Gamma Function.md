#lect3 
The generalized factorial function
$$\Large \Gamma(\alpha) = \int_0^\infty w^{\alpha-1}e^{-w}dw$$
##### Properties  of Gamma Function:
 1. $\Gamma(1) = 1$
 2. $\forall\alpha > 1$,   $\Gamma(\alpha) = (\alpha-1)\Gamma(\alpha-1)$
 3. $\forall \alpha \in \mathbb{Z}\text{ and }\alpha > 0$,  $\Gamma(\alpha) = (\alpha -1)!$
 4. $\Gamma(\frac{1}2) = \sqrt{\pi}$ 

#### In R
```R
# P(X<=x)
pgamma(x,alpha,lambda)

# P(2<=X<=5)
pgamma(5,alpha.lambda) - pgamma(2,alpha,lambda)

```

#### Variance of Gamma Function
$$\large X\sim Ga(\alpha,\lambda)$$$$\large E(x)=\mu=\frac{\alpha}{\lambda}$$$$\large Var(x) = \sigma^2 = \frac{\alpha}{\lambda^2}$$
#### Some formula that I don't get
$$\large X \sim Ga(\alpha, \lambda)$$$$\large f(x) = \frac{\lambda^{\alpha}}{\Gamma(\alpha)}x^{\alpha-1}, x\ge0$$
