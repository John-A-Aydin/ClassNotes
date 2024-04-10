==**16.4**==
# Defn
Let $\large C$ be a smooth, [[Positively or Negatively Oriented Curve|positively oriented]], [[Jordan Curve]] that encloses a 2d region $\large D$.
Then if $\large \vec{F}(x,y) = \langle M(x,y), N(x,y) \rangle$ is differentiable on $\large D$, then
$$\large \oint_{C} \vec{F} \cdot d \vec{r} = \oint_{C}M\; dx + N\; dy = \int\int_{D}\Big(\frac{\partial N}{\partial x} - \frac{\partial M}{\partial y} \Big) \; dA$$

==Green's Theorem can only be applied to closed curves!!!!!==

### What happens if the [[Vector Fields|vector field]] is conservative?

$$\large W = \int \int_{D} \left(\frac{\partial N}{\partial x} - \frac{\partial M}{\partial y}\right)dA = 0$$

# Examples
### Example 1

Let $\large C$  be the boundary of the triangle with the vertices
$\large ( 0 , 0 )$
$\large (  1 , 2 )$
$\large ( 0 , 2 )$

Find
$$\large \oint_{C} 4x^{2}y\; dx + 2y \; dy$$

##### Without Green's
Since this curve forms a triangle it can be broken up into 3 pieces
We would have to compute the [[Line or Path Integral|line integral]] for each of these 2 curves.

##### With Green's
$$\large \oint_{C} 4x^{2}y\; dx + 2y \; dy = \int \int_{D} (0-4x^{2})\; dA$$
where $\large D$ is the region enclosed by $\large C$
Now we just have to find the bounds for the [[Non-Rectangular Regions|double integral]]
$$\large -4\int \int_{D}x^{2} \; dA = -4\int_{0}^{1}\int_{2x}^{2} x^{2} \; d y \; d x = - \frac{2}{3}$$

### Example 2

Let $\large C$ be any smooth [[Jordan Curve]] with [[Positively or Negatively Oriented Curve|positive orientation]] enclosing $\large D$
Find
$$\large \oint_{C}- \frac{y}{2}\; dx + \frac{x}{2}\; dy$$
By Green's Theorem:
$$\large \oint_{C}- \frac{y}{2}\; dx + \frac{x}{2}\; dy = \int\int_{D} \left(\frac{1}{2}\right) - \left(- \frac{1}{2}\right) \; dA = \int \int_{D} 1 \; dA$$

This shows that the integral is just the area of $\large D$

### Example 3
Evaluate
$$\large \oint_{C} (x^{3} + 2y)\; dx + (4x - 3y^{2}) \; dy$$
Where $\large C$ is the ellipse
$$\large \frac{x^{2}}{a^{2}} + \frac{y^{2}}{b^{2}} = 1$$
By Green's Theorem:
$$\large \oint_{C} (x^{3} + 2y)\; dx + (4x - 3y^{2}) \; dy = \int \int_{D} 4-2 \; dA = 2 \int \int_{D} 1 \; dA$$
This integral ends up being double the area of the elipse.
$$\large \text{Area of an elipse} = \pi a b$$
so the answer is
$$\large 2 \pi a b$$


