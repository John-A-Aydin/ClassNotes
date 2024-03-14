**==15.5==**

$$\Large \int \int \int_{R}f(x,y,x)dV \text{ , } R = \text{3D region}$$

In a triple integral with $\large z$ bounded by the functions

$\large g_{1}(x,y) \le z \le g_{2}(x,y)$, 

We need to look at the 2 dimensional projection cast on the x-y plane, $\large R_{xy}$

On this projection, $\large x$ and $\large y$ are bounded by

$\large h_{1}(y) \le x\le h_{2}(y)$

$\large c \le y \le d$

==In general we start with the variable that is dependent on the most variables==

This gives

$$\large \int_{c}^{d}\int_{h_{1}(y)}^{h_{2}(y)}\int_{g_{1}(x,y)}^{g_{2}(x,y)} f(x,y,z) dz \text{ }dy \text{ }dx$$

In this class outer limits of integration will <u>always</u> be constants


### Example 1

Evaluate

$\large \int_{-2}^{5}\int_{0}^{3x}\int_{y}^{x+2} \text{ }4 \text{ }dz \text{ }dy \text{ }dx$

Notice that the upper and lower bounds of the innermost integral are only functions of one variable, but are still considered functions of x and y.

$\large = 4 \int_{-2}^{5}\int_{0}^{3x}x+2-y dy dx$

$\large= 4\int_{-2}^{5} 3x^{2} +6x - \frac{1}{2}(3x)^{2} dx$

...

$\large = -14$


### Example 2

Find the volume of the region enclosed by

$\large z = x^{2} +3y^{2}$  and $\large 8-x^{2}-y^{2}$

Since our information is given in the form $\large z = f_{1}(x,y)$ and $\large z = f_{2}(x,y)$ the innermost integral  will be $\large z$

To get the other 4 limits of integration we need to figure out the curve(s) that define the projection on the x-y plane

Since $\large z=z$ we can just set the two functions of x and y equal to each other to find their intersections.

$\large x^{2} + 3x^{2} = 8-x^{2}-y^{2} \Leftrightarrow x^{2}+2y^{2} = 4$

This tells us that the projection is an ellipse.

![[tripple-int-ex2.png]]

Notice that this region is both horizontally and vertically simple. This means we can use either order for the outside integrations.

We will arbitrarily choose to see it as horizontally simple region. So

$\large -\sqrt{4-2y^{2}} \le x \le \sqrt{4-2y^{2}}$

and

$\large -\sqrt{2} \le y \le  \sqrt{2}$

So the final integral that we need to compute is:

$$\large \int_{-\sqrt{2}}^{\sqrt{2}} \int_{-\sqrt{4-2y^{2}}}^{\sqrt{4-2y^{2}}}\int_{x^{2} +3y^{2}}^{8-x^{2}-y^{2}} 1 \text{ }dz \text{ }dx \text{ }dy = 8 \pi \sqrt{2}$$
### Example 3*

Find the volume of the pyramid (tetrahedron) $\large D$ with vertices at
$\large (0,0,0)$
$\large (0,1,0)$
$\large (1,1,0)$
$\large (0,1,1)$

![[pyramid-ex3.png]]

Since $\large D$ is a pyramid, its faces are [[Planes|planes]]
and we can find the equations of these planes because we have three points for each one

back face: $\large x=0$
bottom face: $\large z=0$
right face: $\large y=1$

left face: 
plane that contains
$\large (0,0,0)$
$\large (0,1,1)$
$\large (1,1,0)$

$\large x-y+z = 0$
See the example in [[Planes]] for work

$\large \text{Volume} = \int\int \int_{D}1 \; dV$

#### 1. Integrate z first

The projection $\large D_{xy}$ is in the x-y plane

![[pyramid-ex3-projection.png]]

This triangle is bounded by the equations
$\large y=1$
$\large x=0$
$\large y=x$

This gives two possible orders of integration
$$\large \int_{0}^{1}\int_{x}^{1}\int_{0}^{y-x} 1 \; d z \; d y \: d x\tag{1}$$
and
$$\large \int_{0}^{1}\int_{0}^{x}\int_{0}^{y-x} 1 \; d z \; d x \: d y\tag{2}$$

#### 2. Integrate x first

The projection $\large D_{yz}$ is in the y-z plane

![[x-first-pyramid-ex.png]]

This projection is bounded by  the lines:
$\large y = 1$
$\large z = 0$
$\large y=z \Leftrightarrow z=y$
This gives us another two orders
$$\large \int_{0}^{1}\int_{z}^{1}\int_{0}^{y-z} 1 \; d x \; d y \: d z \tag{3}$$
and 
$$\large \int_{0}^{1}\int_{0}^{y}\int_{0}^{y-z} 1 \; d x \; d z \: d y \tag{4}$$
#### 3. Integrate y first

The projection $\large D_{xz}$ is in the x-z plane

![[y-first-pyramid-ex.png]]

From this projection we see that the shape is bounded by the lines
$\large x= 0$
$\large z= 0$
$\large z = 1-x \Leftrightarrow x = 1-z$

$$\large \int_{0}^{1}\int_{0}^{1-z}\int_{x+z}^{1} 1 \; d y \; d x \: d z \tag{5}$$
and
$$\large \int_{0}^{1}\int_{0}^{1-x}\int_{x+z}^{1} 1 \; d y \; d z \: d x\tag{6}$$

