#lect6

If we have Z,  a normal distribution
and V a [[Chi-Square Distribution]] with k degrees of freedom,

The Student's t-Distribution is:
$$\large T = \frac{Z}{\sqrt{V/k}}$$ **Mean: 0
**Variance: $\large k(k-2)$

As the degrees of freedom (k) increases, it approaches a [[Normal Distribution]]

### Applying this to a [[Normal Population]]
$$\large T = \frac{\hat{X}-\mu}{S/\sqrt{n}}$$
This is a t-Distribution with $\large k = n-1$ degrees of freedom

Knowing that the degrees of freedom is proportional to n, with higher n, the t-Distribution will get closer to a [[Normal Distribution]]

The 95% CI for the T distribution
$$\large[\hat{X} \pm (t_{n-1;0.025})\frac{S}{\sqrt{n}}]$$ where $\large t_{n-1;0.025}$ is

```R
qt(0.975, n-1)
```

an $\large n \rightarrow \infty$, qt(0.975, n-1) $\large  \rightarrow 1.96$ 

#### Creating a CI in R
```R
# Creates a 95% CI for the pop mean for the given sample
t.test(sample)

# Creating a 99% CI
t.test(sample, conf.level = 0.99)
```
