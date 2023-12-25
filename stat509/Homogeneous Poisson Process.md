
HPP(x)

See [[Poisson Variable]] for RStudio code with explanations 

$N(t)$ - number of events that occur in the interval of \[0,t]
### Conditions for HPP()
1. $N(0) = 0$
2. $N(t) \approx POI(\lambda t)$
	$P(N(t)=k) = \frac{e^{-t\lambda}(\lambda t)^k}{k!}$
3. .
4. $N(s,t)\approx POI(\lambda(t-s))$

It takes an average of $\large \frac{1}{\lambda}$ to get to the first event 
### Ex.

The event is an insurance claim at State Farm

$\large \lambda = 5$ claims/month

1. What is the probability of 0 claims in the first two months?
	$P(N(2) = 0)$ 
	$N(2) \approx POI(2\lambda = 10)$
	We can use dpois()

2. What is the probability of at least 10 claims in the first two months?
	$= P(N(2) \ge 10)$
	$= 1-P(N(2)\lt 10)$
	$= 1-P(N(2)\le 9)$
	We can use ppois(9, 10) in R
	$= 1- ppois(9, 10)$

3. What is the probability that the first event occurs on or or before 5 months
	$= P(N(5)\ge 1)$
	$= 1 - P(N(5) = 0)$
	Using R,
	$= 1-dpois(0, 25)$

### Time to the occurrence of the first event

Probability that the first event will occur on or before $t$

$\large F_T(t) = P(T\le t)$$
$\large = P(N(t)\ge 1)$
$\large = 1- P(N(t) = 0)$
$\large= 1 - e^{-\lambda t}$
