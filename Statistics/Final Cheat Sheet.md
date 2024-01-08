COV = $\sigma_{xy} = E(xy)- (\mu_x)(\mu_y)$ 
or
$Cov(X,Y) = E\{XE[Y|X]\} - E(X)E(Y)$
VAR = $E(x^{2})-\mu^{2}$
CORR = $\frac{\sigma_{XY}}{\sigma_{X}\sigma_{Y}}$

##### HPP
$P\{T\le t\} = 1-e^{-\lambda t}$
Time to first event = $\frac{1}{\lambda}$
$P(N(t) = k) = \frac{e^{-t \lambda}(\lambda t)^k}{k!}$
$P(X=x) = \frac{e^{-\lambda}\lambda^x}{x!}$

##### Sampling
$\mu_{\bar{X}} = E(\bar{X})= \mu$ 
$\sigma^{2}_{\bar{X}} = Var(\bar{X}) = \frac{\sigma^2}{n}$
$\sigma_{\bar{X}}= SE(\bar{X}) = \frac{\sigma}{\sqrt{n}}$ 
$E(\bar{X}^{2})= (\frac{\sigma^2}{n}+\mu^2)$
**Normal Conf Int**
$\text{Conf Int} = Z \frac{S}{\sqrt{n}}$

**Bernoulli**
$L(\theta)=\theta^{T}(1-\theta)^{n-T}$
$SD(\hat\theta) = SE(\hat\theta) = \sqrt{\frac{\theta(1-\theta)}n}$
$ME(\hat{X})=1.96\hat{SE(\bar{X})} = 1.96\sqrt{\frac{\bar{X}(1-\bar{X})}{n-1}}$

##### Bayes Theorem
$P(A_j|B) = \frac{P(A_j)P(B|A_j)}{\sum^n_{i=1}P(A_i)P(B|A_i)} = \frac{P(A_j)P(B|A_j)}{P(B)}$

##### Combination & Permutation
$_{N}C_k=\Big( ^N_k \Big)= \frac{N!}{k!(N-k)!}$
$_{N}P_k = \frac{N!}{(N-k)!}$

##### Conditional Prob
$P(A|B) = \frac{P(A\cap B)}{P(B)}$

$P(A\cap B) = P(A)P(B|A)$

##### LRM
$\alpha = \mu_{Y}-\beta \mu_{X}$
$\beta= \rho \frac{\sigma_{Y}}{\sigma_{X}}=\frac{\sigma_{XY}}{\sigma^{2}_{X}}$

