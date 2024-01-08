Sample Statistics - data that can be calculated only with the sample data
## Sampling of a Discrete Variable

##### The joint pmf:
$\large p(x_1, x_2, \text{ ... },x_n; \theta) = \prod_{i=1}^np(x_i;\theta)$ 

##### Likelihood of a given $\theta$
Represents the likelihood of getting the data seen in the sample with the given $theta$ 
$\large L(\theta) = \prod_{i=1}^np(x_i;\theta)$


## Sampling from a Normal Population

$\large X_1, X_2, \text{ ... }X_n$   $\large N(\mu, \sigma^2)$

##### Likelihood Function
	$\large L(\mu, \sigma^2) = \frac{1}{(\sigma^2)^{(n/2)}(\sqrt{2\pi})^n}exp(-\frac{1}{2\sigma^2}\sum^n_{i=1}(x_i-\mu)^2)$

$\large \bar{X} = \frac{1}{n}\sum\limits_{i=1}^{n}X_{i}$  

## Sampling from an Exponential Population

$\large f(t;\lambda)=\lambda\exp(-\lambda t)$ 

$\large X_{1}, X_{2},\text{ ... }X_{n}$   


## Sample Statistics in R

```R
# Create Vectors
x <- c(1,2,3,4)
y <- c(1,2,3,4)

# Create Histogram
hist(x)

# Find mean
mean(x)

# Find variance
var(x)

# Find standard deviation
sd(x)

# Find mean
median(x)

# Find covariance
cov(x, y)

# Find correlation
cor(x, y)

```

## General Formulas (Central Limit Theorem)

$\large\mu_{\bar{X}} = E(\bar{X})= \mu$ 

$\large \sigma^{2}_{\bar{X}} = Var(\bar{X}) = \frac{\sigma^2}{n}$

$\large\sigma_{\bar{X}}= SE(\bar{X}) = \frac{\sigma}{\sqrt{n}}$ 

$\large E(\bar{X}^{2})= (\frac{\sigma^2}{n}+\mu^2)$


#### Confidence Interval of $\mu$ 

Tells us a range of values that the population mean could be based on our sample data with a certain percent probability

