$$\Large p_{Y|X}(Y|X) = P(Y=y|X=x) = \frac{p(x,y)}{p_x(x)}$$$$\Large p(x,y) = p_x(x)p_{y|x}(y|x) = p_y(y)p_{x|y}(x|y)$$
## Conditional [[Probability Density Function (PDF)|PDF]]
- Probability density function of one variable when the value of the other variable is fixed

## Conditional [[Probability Mass Function (PMF)|PMF]]
- Probability mass function of one variable when the value of the other variable is fixed

#### [[Theorem of Total Probability]]
$$\Large p_Y(Y) = P(Y=y) = \sum_xp_x(x)p_{y|x}(y|x)$$
#### [[Bayes Theorem]]
$$$$

### Iterated Rules
Work for both discrete and continuous 
$$\large E(Y) = E\{E[Y|X]\}$$Average of conditional averages gives us the average of Y
$$\large E(Y^2) = E\{E[Y^2|X]\}$$$$\large Var(Y) = E[Var(Y|X) + Var[E(Y|X)]$$$$E(XY) = E\{XE[Y|X]\}$$
$$Cov(X,Y) = E\{XE[Y|X]\} - E(X)E(Y)$$or $$Cov(X,Y) = Cov\{X,E(Y|X)\}$$
