##### Ex.
We have N balls, with R red balls and N-R blue balls 
X is the number of red balls in the sample of balls we pick at random without replacement

Proportion of Reds: $$\frac{R}N$$
Proportion of Blues: $$\frac{N-R}N$$
$$P(X=x)=p(x)=\Big(^n_x\Big)\Big(\frac{R}{N}\Big)^x\Big(\frac{N-R}{N}\Big)^{n-x}$$

##### Ex.
Same principles where we flip a coin twenty times
X is the number of heads we get $$P(X=x)=\Big(^{20}_x\Big)\Big(\frac{1}{2}\Big)^x\Big(\frac{1}{2}\Big)^{20-x}$$
### In R
```R
# Calculating the probability of exactly k
dbinom(k, n, p)

# Calculating the probability of at most k
pbinom(k, n, p)
```
**Where:**
	*k* is the target number
	*n* is the total number of trials
	*p* is the probability of what we are counting


```R
X <- BIN(n, theta)
u <- n*theta
variance <- n*theta*(1-theta)
```