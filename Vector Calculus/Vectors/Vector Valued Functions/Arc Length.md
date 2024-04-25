<<<<<<< HEAD
  L    et $\large C$ be a curve that is parameterized by a [[Vector-Valued Function]]
=======
oLet $\large C$ be a curve that is parameterized by a [[Vector-Valued Function]]
>>>>>>> 77dc23754e5a40d1bdb7ae0c55abf259c000f96d
$\large \vec{r}(t) = \langle x(t), y(t) \rangle$,    $\large a \le t \le b$

How do we find the linear distance covered by this curve $\large C$ for $\large a \le t \le b$?

In Calc II we might have seen:
$$\large L = \int_{a}^{b} \sqrt{[x'(t)]^{2} + [y'(t)]^{2}} \; d t$$

This is the arc length formula for a 2d curve. If we apply this to a vector valued function we get:
$$\large L = \int_{a}^{b} ||\vec{r}'(t)|| \; d t$$
This definition extends to curves of higher dimensions.

### Example 1

Find the length of the curve
$\large \vec{r}(t) = \langle \cos(t), \sin(t), t \rangle$
from the point $\large ( 1 , 0 , 0 )$  to $\large ( 1 , 0 , 2\pi )$

$\large L = \int_{a}^{b} ||\vec{r}'(t)|| \; d t$

We are not given $\large a$ or $\large b$ so we need to use the VVF to find the values of $\large t$ we need.
$\large 0 \le t \le 2\pi$

$\large \vec{r}'(t) =\langle -\sin(t), \cos(t), 1 \rangle$

$\large ||\vec{r}'(t)|| = \sqrt{\sin^{2}(t) + \cos^{2}(t)+ 1} = \sqrt{2}$

so

$\large L = \int_{0}^{2\pi} \sqrt{2} \; d t = 2\pi\sqrt{2}$ 
