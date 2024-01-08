#lect5
A population where a binary value is measured 

$\theta$ denotes the proportion of 1's
$1-\theta$ denotes the proportion of 0's

## Sampling from a Bernoulli Population

If we have a Bernoulli population that is sufficiently large,  we treat it as with replacement

#### Things to know
$L(\theta)$  = Likelihood of theta being representative of the entire population
$T$      = number of 1's in the sample

#### Finding a value of $\theta$
[[Likelihood Function]] of $\theta$:   $L(\theta)$ 
$\large L(\theta) = \Pi^n_{i=1}\theta^{x_i}(1-\theta)^{1-x_i}$
or
$\large L(\theta)= \theta^{T}(1-\theta)^{n-T}$
where 
$T = \sum\limits_{1}^{n}X_{i}$


### How to use T to learn about $\theta$

#### Estimating the mean
$\large \bar{X} = \frac{T}{n} =$ proportion of 1's in the sample $\large = \hat\theta$ 

$\large E(\hat\theta) = E(\frac{T}n = \frac{1}nE(T) = \frac{n\theta}n = \theta$ 

$\large Var(\hat\theta) = Var(\frac{t}n = \frac{1}{n^2}Var(T) = n\theta(1-\theta)/n^2 = \frac{\theta(1-\theta)}n$ 

$\large SD(\hat\theta) = SE(\hat\theta) = \sqrt{\frac{\theta(1-\theta)}n}$    - standard error

If we apply [[Chebyshev's Inequality]] to this problem, we see that $\hat\theta \rightarrow^{PR} \theta$  as $n\rightarrow \infty$ 

#### Margin of Error
$ME(\hat{X})=1.96\hat{SE(\bar{X})} = 1.96\sqrt{\frac{\bar{X}(1-\bar{X})}{n-1}}$

#### Confidence interval for $\hat\theta$


Suppose we want the length of the interval to be no more than 2d 

$\Large n \ge \frac{(Z_{\alpha/2})^2\hat\theta(1-\hat\theta)}{d^2}$ 

$\hat\theta(1-\hat\theta)$ is max at $\hat\theta = 1/2$ 

$\Large n \ge \frac{(Z_{\alpha/2})^2}{4d^2}$ 

### Mean and Variance

$\Large\mu= \theta$

$\Large\sigma^{2} = (1-\theta)\theta$

## Maximum Likelihood Approach

$\large l(\theta)= logL(\theta) = Tlog(\theta)+(n-T)log(1-\theta)$
