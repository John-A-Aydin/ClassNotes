==**15.4**==

If the region of integration is part of a circle, standard (Cartesian) coordinates are the wrong tool for the job.

### Polar Rectangles

In [[Polar Coordinates|polar coordinates]] we divide the region into "polar rectangles"

$\large R = \{(r,\theta) : a\le r\le b, \alpha \le \theta\le \beta\}$

![[polar-rectangle.png]]

The height of our box is given by:

$\large x = f(x,y) = f(r\cos \theta, r\sin \theta) = F(r, \theta)$

The area of each polar rectangle is given as:

$\large \Delta A_{k} = \Delta r_{k} \Delta \theta_{k}\bar{r}_{k}$

where $\large \bar{r_{k}}$ is the average radius of polar rectangle k

The volume of a single polar box is:

$\large \Delta V_{k} = F(r_{k}^{*}, \theta_{k}^{*})\Delta A_{k}$

$\large \Delta V_{k} = F(r_{k}^{*}, \theta_{k}^{*})\Delta r_{k} \Delta \theta_{k}\bar{r}_{k}$

# Integral

Adding up all of these boxes and letting n-> $\infty$ we get

$$\Large V = \int \int_{D}f(x,y)dA = \int \int_{D^{*}}F(r,\theta)r\text{ }drd \theta $$

where $\large D^{*}$ is the polar version of $\large D$

**Remember!**
	$\large x = r \cos \theta$
	$\large y = r \sin \theta$
	$\large dA \rightarrow r \text{ } drd \theta$


### Example 1

Find the volume of the solid whose base is
$\large R = \{(r,\theta): 1\le r \le 3, 0\le \theta\le \frac{\pi}{4}\}$

and who's top is 
$\large z = e^{x^{2}+y^{2}}$

First convert the equation to polar form.

$\large z = e^{r^{2}(\cos^{2}\theta+\sin^{2}\theta)} = e^{r^{2}} = F(r, \theta)$

since $\large \cos^{2}\theta +\sin^{2}\theta=1$

Now we have to set up the integral.

$\Large \int_{0}^{\frac{\pi}{4}}\int_{1}^{3}e^{r^{2}}r \text{ }drd \theta$

$\large = \frac{1}{2} \int_{0}^{\frac{\pi}{4}}e^{r^{2}} |^{3}_{1} d \theta$

$\large= \frac{e^{9} -e}{2}\int_{0}^{\frac{\pi}{4}}1 d \theta$

$\large = \frac{e^{9}-e}{2}\frac{\pi}{4}$

### Example 2 ==IMPORTANT==

Evaluate 

$\large \int_{0}^{1}\int_{0}^{\sqrt{1-x^{2}}} x^{2}+y^{2} dydx$

If we attempt to use Cartesian coordinates this will take trig substitution

![[polar-integral-example.png]]

Looking at the bounds of integration, we can see that this is just a quarter of the unit circle.

Switching to polar coordinates gives:

$\large x^{2} + y^{2} = r^{2}(\cos^{2}\theta+\sin^{2}\theta) = r^{2} = F(r, \theta)$

$\large 0\le r\le 1$

$\large 0 \le \theta\le \frac{\pi}{2}$

$\large dydx \rightarrow r \text{ }drd \theta$

So we get:

$\Large \int_{0}^{\frac{\pi}{2}}\int_{0}^{1}r^{2} r \text{ }drd \theta$

...

$= \frac{\pi}{8}$