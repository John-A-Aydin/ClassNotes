==**16**==

Generalization of
$$\large \int_{a}^{b} f(x) \; d x$$
Think of $\large [a, b]$  as a path $\large C$ from $\large x=a$  to $\large x=b$

Now, let $\large C$ be any 2d (planar) curve given by
$\large \vec{r}(t) = \langle x(t), y(t) \rangle$

$\large C$ starts at $\large ( x(a) , y(a) )$  and stops at $\large ( x(b) , y(b) )$
How do we integrate a function $\large f(x,y)$ along $\large C$?

##### Notation:
$$\large \int_{C} f(x,y) \; d S$$
where $\large dS$ represents the [[Arc Length|arc length]].
![[Line or Path Integral.png]]

This is the area of a surface whose shape is defined by the path under $\large f(x,y)$ defined by $\large C$

The overall idea of the integral is splitting this path into small partitions $\large dS$
These partitions have two components:
$\large dx$: The change in x from one side to the other
$\large dy$: The change in y from one side to the other

$\large dS$, $\large dx \text{ , } dy$ form a right triangle so:
$\large dS = \sqrt{(dx)^{2}+(dy)^{2}}$

$\large dS = \sqrt{(\frac{dx}{dt})^{2} + (\frac{dy}{dt})^{2}}\;dt \Rightarrow dS = ||\vec{r}'(t)||dt$

$$\Large \int_{C} f(x,y) \; d S = \int_{a}^{b} f(x(t), y(t)) \; \sqrt{[x'(t)]^{2} + [y'(t)]^{2}}\; dt$$

### Example 1

Evaluate
$$\large \int_{C} x^{2}y \; d S$$
where $\large C$ is given by
$\large x(t) = 3 \cos(t)$
$\large y(t) = 3 \sin(t)$
$\large 0 \le t \le \frac{\pi}{2}$

$$\large \int_{C} f(x,y) \; d S = \int_{0}^{\frac{\pi}{2}} 81 \cos^{2}(t)\sin(t) \; d t = 27$$


