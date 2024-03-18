==**15.7**==

Spherical coordinates are in the form
$$\large P = ( \rho , \phi , \theta )$$
where $\large \theta$ is the angle on the x-y plane from the x-axis,
$\large \rho$ is the distance from the origin to the point,
$\large \phi$ is the angle from the positive z-axis to the line segment connecting the origin and $\large P$

![[Vector Calculus/attachments/Regions Defined by Spherical Coordinates.png]]

These properties give us a range for each of these variables
$\large 0 \le \rho$
$\large 0 \le \theta \le 2\pi$
$\large 0 \le\phi \le \pi$

### Converting to Spherical Coordinates

$\large x \Rightarrow \rho \sin\left(\phi\right) \cos\left(\theta\right)$
$\large y \Rightarrow \rho \sin\left(\phi\right)\sin\left(\theta\right)$
$\large z \Rightarrow \rho \cos\left(\phi\right)$
$\large dV \Rightarrow \rho^{2} \sin\left(\phi\right) \; d \rho \; d \phi \; d \theta$

### Example 1

Find the volume of a sphere of radius $\large R$

$$\large Vol(S) = \int \int \int_{S} 1 \; d V \Rightarrow \int_{0}^{2\pi}\int_{0}^{\pi}\int_{0}^{R} \rho^{2}\sin\left(\phi\right) \; d \rho \; d \phi \: d \theta$$

$\large = \frac{R^{3}}{3} \int_{0}^{2\pi}\int_{0}^{\pi} \sin(\phi) \; d \phi \; d \theta$

$\large = \frac{2R^{3}}{3} \int_{0}^{2\pi} 1 \; d \theta$

$\large = \frac{4}{3} \pi R^{3}$

### Example 2

Find the volume of the region $\large R$ cut from the sphere of radius 1 by
$\large \phi = \frac{\pi}{3}$

Note that when $\large \phi$ is set to a constant it forms a cone
$$\large \text{Volume} = \int_{0}^{2\pi}\int_{0}^{\frac{\pi}{3}}\int_{0}^{1} \rho^{2}\sin(\phi)\; d \rho \; d \phi \: d \theta$$
### Example 3

Evaluate:
$$\large \int_{0}^{3}\int_{0}^{\sqrt{9-x^{2}}}\int_{0}^{\sqrt{9-x^{2}-y^{2}}} xy \; d z \; d y \: d x$$
First we should try to visualize the region of integration

The limits of integration of $\large z$ form a hemisphere
$\large z = \sqrt{9-x^{2}-y^{2}} \Leftrightarrow x^{2}+y^{2}+z^{2} = 9$

![[Regions Defined by Spherical Coordinates 1.png]]

This shows that this is a sphere with center at the origin and radius 3.

The x and y limits of integration form a quarter circle.
$\large y=\sqrt{9-x^{2}} \Leftrightarrow 9 = x^{2}+y^{2}$
$\large 0\le x \le 3$

![[Regions Defined by Spherical Coordinates-1.png]]

Since we know the shape, we can now convert to spherical coordinates giving:
$$\large \int_{0}^{\frac{\pi}{2}}\int_{0}^{\frac{\pi}{2}}\int_{0}^{3} (\rho \sin(\phi)\cos(\theta))*(\rho\sin(\phi)\sin(\theta))*\rho^{2}\sin(\phi) \; d \rho \; d \phi \: d \theta$$
$$\large = \int_{0}^{\frac{\pi}{2}}\int_{0}^{\frac{\pi}{2}}\int_{0}^{3} \rho^{4} \sin^{3}(\phi) \cos(\theta)\sin(\theta) \; d \rho \; d \phi \: d \theta$$
Now we just evaluate the integral normally
**Hint:**
$\large \int\sin^{3}(\alpha)\;d \alpha = \frac{1}{3}\cos^{3}(\alpha)-\cos(\alpha)$

How would this change if the original region of integration was
$$\large \int_{0}^{3}\int_{-\sqrt{9-x^{2}}}^{\sqrt{9-x^{2}}}\int_{0}^{\sqrt{9-x^{2}-y^{2}}} xy \; d z \; d y \: d x$$
Ans: It would change the limits of $\large \theta$ to $\large -\frac{\pi}{2} \le \theta \le \frac{\pi}{2}$

![[Regions Defined by Spherical Coordinates-2.png]]

What if it was:
$$\large \int_{0}^{3}\int_{0}^{\sqrt{9-x^{2}}}\int_{-\sqrt{9-x^{2}-y^{2}}}^{\sqrt{9-x^{2}-y^{2}}} xy \; d z \; d y \: d x$$

The limits of integration of $\large \phi$ will change to $\large 0 \le \phi \le\pi$
![[Regions Defined by Spherical Coordinates 2.png]]


### Example 4

Find the volume of the solid that is between two spheres centered at the origin of radii 3 and 5
This tells us that:
$\large 3 \le \rho \le 5$
$\large 0 \le \phi \le \pi$
$\large 0 \le \theta \le 2\pi$

This gives the integral:
$$\large \int_{0}^{2\pi}\int_{0}^{\pi}\int_{3}^{5} \rho^{2}\sin(\phi) \; d \rho \; d \phi \: d \theta$$


### Example 5

Evaluate
$$\large \int \int \int_{D} x^{2}+y^{2}+z^{2}dV$$
Where $\large D$ is

Converting to spherical coordinates:
$$\large x^{2} +y^{2}+z^{2} \Rightarrow (\rho \sin(\phi)\cos(\theta))^{2} + (\rho \sin(\phi)\sin(\theta))^{2} + (\rho \cos(\phi))^{2}$$
This new equation simplifies to 
$$\large \rho^{2}$$


