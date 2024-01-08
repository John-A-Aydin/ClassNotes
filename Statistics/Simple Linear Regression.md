Analysis of the two variables $X$ and $Y$
$$\large Y = \text{response or dependent variable}$$$$\large X = \text{covariates, predictors, control, or independent variables}$$
## Creating a linear prediction of $Y$
**There is a linear model if $Y$ satisfies**
$$\large\mu_{Y|x}= E[Y|X=x] = \alpha + \beta x$$
Where$$\large\alpha = \mu_{Y}-\beta \mu_{X}$$$$\large\beta= \rho \frac{\sigma_{Y}}{\sigma_{X}}=\frac{\sigma_{XY}}{\sigma^{2}_{X}}$$
## Sample to SLR
The sample data will be a set of order pairs.
$$\large Y_{i} = \alpha+\beta X_{i}+ \epsilon_{i}$$
Where [[Normal Distribution|]]  
$$\large \epsilon_{i} \approx N(0, \sigma^{2})$$
If the variance of Y does not depend on X, the data is homeostatic or smth

We want to make the difference between the sample points and the line as small as possible.
### Least-Squares Estimation
$$\large Q(a, b) = \sum\limits_{i=1}^{n} [Y_{i} - (a + b X_{i} )]^{2}$$
To get the estimates of $\alpha$ and $\beta$ we equate the derivatives to 0
$$\large\frac{\delta Q}{\delta a} \text{ and } \frac{\delta Q}{\delta b}$$

This ends up giving us
$$\large a = \bar{Y} - b\bar{X}\text{ and } b = r \frac{S_{Y}}{S_{X}} $$$$\large\hat{Y}(x) = a + bx$$ We can also get and Unbiased Estimator of $\large\hat{\sigma}^{2}$ with
$$\large \frac{1}{n-2} \sum\limits_{i=0}^{n} [Y_{i} - \hat{Y_{i}}]^{2?}$$
#### Coefficient of Determination ($R^{2}$)
$$\large R^{2} = [cor(Y_{i},\hat{Y_{i}})]^{2}$$
If it is close to 1 the predictor is good, close to 0 and its bad


## In R
```R
# Do calculations on set
outlm = lm(Y~X)

# How we get a and b and other data
summary(outlm)

# How to get a and b
outlm$coefficients 

outlm$fitted.values

# Plot the data and superimpose the line of best fit
plot(X, Y)
lines(X, outlm$fitted.values) 
# or 
abline(outlm)

# Alternatively
r = cor(X,Y)
sy = sd(Y)
sx = sd(X)
my = mean(Y)
mx = mean(X)

b = r*sy/sx
a = my - b*mx
```

### Making Inferences

If $\large \beta = 0$, we can say that X doesn't effect Y
$$\large \mu_{b}= \beta $$$$\large\sigma_{b}^{2} = ??$$ 