We want to measure the rate of change of $\large f(x,y)$ in <u>any</u> given direction.

To do this we use a [[Unit Vector|unit vector]] $\large \vec{u}$

#### Def.

Let $\large z = f(x,y)$ be a surface with $\large P_{0} = (x_{0}, y_{0}, z_{0})$ a point on the surface and $\vec{u} = <u_{1}, u_{2}>$ a unit vector

The the directional derivative of $\large f$ in the direction $\vec{u}$at any  point is given by
$$\Large D_{\vec{u}}f(x,y) = lim_{h\to 0}\frac{f(x+hu_{1}, y+hu_{2})-f(x,y)}{h}$$ At a given point $\large (x_{0}, y_{0})$,
$$\Large\Large D_{\vec{u}}f(x_{0},y_{0}) = lim_{h\to 0}\frac{f(x_{0}+hu_{1}, y_{0}+hu_{2})-f(x_{0},y_{0})}{h}$$
This is really just a generalization of $\large f_{x}$ and $\large f_{y}$
$$\Large f_{x}(x,y) = lim_{h\to0}\frac{f(x+h, y) - f(x,y)}{h} = D_{\vec{i}}f(x,y)$$
### Theorem

Let $\large f(x,y)$ be differentiable at $\large P_{0} = (x_{0}, y_{0})$

Then $\Large D_{\vec{u}}f(x_{0}, y_{0})= u_{1}f_{x}(x_{0}, y_{0}) + u_{2}f_{y}(x_{0}, y_{0})$

where $\large \vec{u}$ <u>is a unit vector</u>

### Example

Let $\large f(x,y) = 4x^{2}-xy + 3y^{2}$, $\large P_{0} = (2, -1)$ and $\vec{a} = <4,3>$ Find $\large D_{\vec{u}}f(x,y)$  and $\large D_{\vec{u}}f(2,-1)$ 

First we check if the given direction is a unit vector

$\large ||\vec{a}|| = \sqrt{4^{2}+3^{2}} = 5$

so

$\large \vec{u} = <\frac{4}{5}, \frac{3}{5}>$

Note that $\large \vec{u}$ points in the same direction as $\large \vec{a}$

Next we compute the partial derivatives

$\large f_{x} = 8x -y$

$\large f_{y} = -x +6y$

Now find the general directional derivative

$\large D_{\vec{u}}f(x,y) = \frac{4}{5}(8x-y) + \frac{3}{5}(-x+6y) = \frac{29}{5}x + \frac{14}{5}y$

Finally plug in the values of $\large P_{0}$

$\large D_{\vec{u}}f(2,-1) = \frac{44}{5}$



