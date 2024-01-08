#lect3 

$$\Large X\sim N(\mu, \sigma^2)$$$$\large f(x) = \frac{1}{\sigma\sqrt{2\pi}}exp\{-\frac{1}2(\frac{x-\mu}{\sigma})^2\}$$

### In R
```R
#P(X<=x)
pnorm(x,mu,sigma)

# Probability that something is under X standard deviations away from mean?
# didnt rlly explain that well, but look at Ex
pnorm(x) NOT RIGHT

# tells us how many standard dev something is give prob
qnorm(P)

# To find value at a given probability
qnorm(P)*stdDev + mean

```

### Inverse Problem
Find A such that $P(X\le A) = \alpha$ 

$\large \alpha = P(X\le A) = P(Z\le \frac{A-\mu}{\sigma})$ 

qnorm($\alpha$) = $\frac{A -\mu}{\sigma}$  $\Rightarrow$ A = $\sigma$(qnorm($\alpha$)) + $\mu$ 



### Example

X = IQ $\sim N(\mu = 100, \sigma^2 = (15)^2 = 225, \sigma = 15)$
$P(X\le110) = P(Z\le \frac{110-100}{15})= P(Z\le \frac{10}{15}) =$ pnorm(10/15) 


### Transformation of a Normal Variable

$\large Y = Z^2$

What is the dist of Y?

