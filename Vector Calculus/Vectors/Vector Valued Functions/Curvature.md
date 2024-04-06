==**13**==

Let $\large C$ be a curve defined by
$\large \vec{r}(t) = \langle x(t), y(t), z(t) \rangle$,   $\large a \le t \le b$

We know that the [[Derivatives of Vector Valued Functions|derivative]] of $\large \vec{r}(t)$  shows us the direction of the curve and the [[Unit Tangent Vector of VVF|unit tangent vector]] of $\large \vec{r}'(t)$,  $\large \vec{T}'(t)$,  shows //IDK//

Define the scalar function $\large \kappa(t)$ to measure the curvature of $\large C$ at any point along this trajectory.

There are a lot of methods to find this curvature, but we will cover two.

##### Method 1:
$$\large \kappa(t) = \frac{||\vec{T}'(t)||}{||\vec{r}'(t)||}\tag{1}$$

##### Method 2:
$$\large \kappa(t) = \frac{||\vec{r}'(t) \times \vec{r}''(t)||}{||\vec{r}'(t)||^{3}}\tag{2}$$

### Example 1

Find the curvature of
$\large \vec{r}(t) = \langle t, t^{2},t^{3} \rangle$
at any point and at $\large t = 0$

Using Eqn (2)

We only need to deal with finding the derivatives of $\large \vec{r}(t)$ and their [[Cross Product (more info)|cross product]].
This method reduces the amount of magnitudes we need to calculate

$\large \vec{r}'(t) = \langle 1, 2t, 3t^{2} \rangle$
$\large \vec{r}''(t) = \langle 0, 2, 6t \rangle$

$\large \vec{r}'(t) \times \vec{r}''(t) = \langle 6t^{2}, -6t, 2 \rangle$
$\large ||\vec{r}'(t) \times \vec{r}''(t)|| = \sqrt{(6t^{2})^{2} + (-6t)^{2} + 2^{2}} = \sqrt{36t^{4}+36t^{2}+4}$

$\large \vec{r}'(t) = \sqrt{1 + 4t^{2}+9t^{4}}$

so

$\Large \kappa(t) = \frac{\sqrt{36t^{4}+36t^{2}+4}}{(9t^{4}+4t^{2}+1)^\frac{3}{2}}$

### Example 2

Find the curvature of the circle of radius $\large R$

First we need to find $\large \vec{r}(t)$
$\large \vec{r}(t) = \langle R \cos(t), R \sin(t), 0 \rangle$

Using Method 2,

$\large ||\vec{r}'(t)||^{3} = R^{3}$
and
$\large || \vec{r}'(t)\times \vec{r}''(t)|| = R^{2}$

so 
$\large \kappa(t) = \frac{1}{R}$

Since $\large R$ is a constant on a circle, this equation tells us that the curvature of a circle is constant.





