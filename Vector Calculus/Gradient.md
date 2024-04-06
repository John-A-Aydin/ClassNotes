==**14.5**==

The gradient of a scalar function is a [[Vectors|vector]].

# Def.

Let $\large f(x,y)$  be differentiable at a given point $\large (x,y)$ 
with partial derivatives $\large f_{x}(x,y)$, $\large f_{y}(x,y)$

Then the gradient $\large f$, denoted $\large \nabla f$ is the vector:

$$\large \nabla f(x,y) = \langle f_{x}(x,y), f_{y}(x,y)\rangle$$


# Properties of the Gradient

Let $\large f$ and $\large g$ be  differentiable scalar functions and $\large C$ be a scalar value

Then,
$$\large \nabla C = \langle 0,0,0,\text{ ... }, 0\rangle = \vec{0} \ne 0 \tag{1}$$
##### Addition / Subtraction Rule
$$\large \nabla(f \pm g) = \nabla f \pm \nabla g \tag{2}$$
##### Associative Property
$$\large \nabla(Cf) = C \nabla f \tag{3}$$
##### Product Rule
$$\large \nabla (fg) = g \nabla f + f \nabla g \tag{4}$$
##### Quotient Rule
$$\large \nabla \left(\frac{f}{g}\right)= \frac{g \nabla f - f \nabla g}{g^{2}} \tag{5}$$
##### Chain Rule
$$\large \nabla f^{n} = nf^{n-1} \nabla f \tag{6}$$

### Important Property
The gradient can be used to compute [[Directional Derivatives|directional derivatives]] with:
$$\large D_{\vec{u}}f(x_{0},y_{0}) = \nabla f(x_{0}, y_{0})\cdot \vec{u}$$
but we can also use a property of dot products to get
$$\large D_{\vec{u}}f(x_{0}, y_{0})  = ||\nabla f(x_{0}, y_{0})||*||\vec{u}||cos \theta$$
and since the magnitude of a [[Unit Vector|unit vector]] is always 1 we get
$$\large D_{\vec{u}}f(x_{0}, y_{0})  = ||\nabla f(x_{0}, y_{0})||cos \theta$$

This tells us that the directional derivative is as large as possible when $\large cos \theta = 1$ or when $\large \theta = 0$ (when $\large \nabla f$ and $\large \vec{u}$ point in the same direction)

The directional derivative is as small as possible when $\large \theta = \pi$ (when $\large \nabla f$ and $\large \vec{u}$ are pointing in opposite directions) 

### Example

$\large f(x,y) = xe^{y} +x^{2} y$

$\large \nabla f = \langle e^{y}+ 2xy, xe^{y}+2x \rangle$