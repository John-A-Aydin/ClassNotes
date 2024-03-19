==**15.7**==

Spherical coordinates are in the form
$$\large P = ( \rho , \phi , \theta )$$
where: 
$\large \rho$ is the distance from the origin to the point,
$\large \phi$ is the angle from the positive z-axis to the line segment connecting the origin and $\large P$,
$\large \theta$ is the angle on the x-y plane from the x-axis

![[Regions Defined by Spherical Coordinates.png]]

These properties give us a range for each of these variables
$\large 0 \le \rho$
$\large 0 \le \theta \le 2\pi$
$\large 0 \le\phi \le \pi$

### Converting to Spherical Coordinates

$\large x \Rightarrow \phi \sin\left(\phi\right) \cos\left(\theta\right)$
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

Find the volume of the region $\large R$ cut from thee sphere of radius 1 by
$\large \phi = \frac{\pi}{3}$

Note that when $\large \phi$ is set to a constant it forms a cone
$$\large \text{Volume} = \int_{0}^{2\pi}\int_{0}^{\frac{\pi}{3}}\int_{0}^{1} \rho^{2}\sin(\phi)\; d \rho \; d \phi \: d \theta$$
