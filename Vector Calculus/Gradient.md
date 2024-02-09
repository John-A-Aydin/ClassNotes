==**14.5**==

==**A gradient is a [[Vectors|vector]]**==

### Def.

Let $\large f(x,y)$ or $\large f(x,y,z)$  etc.  be differentiable at a given point $\large (x,y)$  or $\large (x,y,z)$ 
with partial derivatives $\large f_{x}(x,y)$, $\large f_{y}(x,y)$

Then the <u>gradient of f</u>, denoted $\large \nabla f$ is the <u>vector</u> 

$$\large \nabla f(x,y) = \langle f_{x}(x,y), f_{y}(x,y)\rangle$$
### Example

$\large f(x,y) = xe^{y} +x^{2} y$

$\large \nabla f = \langle e^{y}+ 2xy, xe^{y}+2x \rangle$

### Properties of the Gradient

Let $\large f$ and $\large g$ be  differentiable scalar functions and $\large C$ be a scalar value

Then,
1. 
	$$\large \nabla C = \langle 0,0,0,\text{ ... }, 0\rangle = \vec{0} \ne 0$$
2. 
	$$\large \nabla(f + g) = \nabla f + \nabla g$$
3. 
	$$\large \nabla(Cf) = C \nabla f$$
4.  Product Rule
	$$\large \nabla (fg) = g \nabla f + f \nabla g$$
5.   Quotient Rule
	$$\large \nabla \left(\frac{f}{g}\right)= \frac{g \nabla f - f \nabla g}{g^{2}}$$
6.  Chain Rule
	$$\large \nabla f^{n} = nf^{n-1} \nabla f$$

### Important Property
With [[Directional Derivatives]] the gradient can be used
$$\large D_{\vec{u}}f(x_{0},y_{0}) = \nabla f(x_{0}, y_{0})\cdot \vec{u} = ||\nabla f(x_{0}, y_{0}||*||\vec{u}||cos \theta = ||\nabla f(x_{0}, y_{0}||cos \theta$$
but we can also use a property of dot products to get
$$\large D_{\vec{u}}f(x_{0}, y_{0})  = ||\nabla f(x_{0}, y_{0})||*||\vec{u}||cos \theta$$
Also notice that the magnitude of a [[Unit Vector|unit vector]] is always 1 so
$$\large D_{\vec{u}}f(x_{0}, y_{0})  = ||\nabla f(x_{0}, y_{0})||cos \theta$$

This tells us that the directional derivative is as large as possible when $\large cos \theta = 1$ or when $\large \theta = 0$ (when $\large \nabla f$ and $\large \vec{u}$ point in the same direction)

The directional derivative is as small as possible when $\large \theta = \pi$ (when $\large \nabla f$ and $\large \vec{u}$ are pointing i opposite directions) 

