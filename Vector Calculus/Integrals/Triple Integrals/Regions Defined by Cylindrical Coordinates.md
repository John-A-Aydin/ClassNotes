==**15.7**==
Cylindrical coordinates are just polar coordinates with $\large z$ tacked on creating a third dimension.

Any given point $\large ( x , y , z )$ has a point directly below it on the x-y plane at $\large ( x , y , 0 )$

$\large x \Rightarrow r \cos\left(\theta\right)$
$\large y \Rightarrow r \sin\left(\theta\right)$
$\large z \Leftrightarrow z$
$\large dz\;dy\;dx \Rightarrow r\;dz\;dr\;d \theta$
so

$\large f(x,y,z) \Rightarrow f ( r \cos\left(\theta\right) , r\sin\left(\theta\right) , z ) = F(r, \theta, z)$

and

$\large \int \int \int_{R} f ( x , y , z ) \; d V \Rightarrow \int \int \int_{R^{*}} F(r,\theta, z)r \; d z \;dr \;d \theta$

### Example 1

Find the volume of the solid in the first [[Octant|octant]] bounded above by the paraboloid 
$\large z = 4-x^{2}-y^{2}$
and laterally by the cylinder
$\large x^{2}+y^{2}=2x$

To find the structure of this shape we need to complete the square of the cylinder to find its shape
$\large x^{2}+y^{2}=2x \Leftrightarrow(x-1)^{2}+y^{2}=1$
so
The circle is centered at $\large ( 1 , 0 )$ and has a radius of 1

![[cylindrical-integral-ex1.png]]

Now that we know the shape we can convert the equations
$\large x^{2}+y^{2}=2x \Leftrightarrow r = 2 \cos\left(\theta\right)$
and
$\large z = 4 -x^{2}-y^{2} \Leftrightarrow z = 4-r^{2}$

The projection on the x-y or $\large \theta$-r plane is a semi circle

$$\large \int_{0}^{\frac{\pi}{2}}\int_{0}^{2 \cos\left(\theta\right)}\int_{0}^{4-r^{2}} 1 \; d z \; d r \: d \theta$$

### Example 2

Compute the triple integral 
$$\large \int \int \int_{D}x^{2}+y^{2}\;dV$$
where $\large D$ is given by 
$$\large \sqrt{x^{2}+y^{2}} \le z\le2$$
Hint: 
$\large \sqrt{x^{2}+y^{2}} = z$  is a cone
and $\large z=2$  is a plane

![[Regions Defined by Cylindrical Coordinates.png]]

Note that this is just the region of integration.

To find the shape of the projection on the x-y plane, we need to set $\large \sqrt{x^{2}+y^{2}} = 2$
This shows us that the projection on the x-y plane is a circle centered on the origin with a radius of 2.

#### Convert to Polar

$\large z = \sqrt{x^{2}+y^{2}} \Rightarrow r$
$\large x^{2}+y^{2} \Rightarrow r^{2}$

so

$$\large \int\int \int_{D} x^{2}+y^{2} \; d V \Rightarrow \int_{0}^{2\pi}\int_{0}^{2}\int_{r}^{2} r^{2}*r \; d z  \; d r  \: d \theta = \frac{16\pi}{5}$$
