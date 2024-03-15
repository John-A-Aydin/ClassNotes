==**15.4**==

If the region of integration is part of a circle, standard (Cartesian) coordinates are the wrong tool for the job.

### Polar Rectangles

In [[Vector Calculus/Definitions/Polar Coordinates|polar coordinates]] we divide the region into "polar rectangles"

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

$\large= \frac{\pi}{8}$

##### What if:

$\large \int_{0}^{1}\int_{\sqrt{1-x^{2}}}^{-\sqrt{1-x^{2}}} x^{2}+y^{2}dy dx$

![[polor-cord-ex-3.png]]

Then in polar coordinates it would be:

$\large \int_{-\frac{\pi}{2}}^{\frac{\pi}{2}}\int_{0}^{1} r^{2}*r drd \theta$

##### Similarly:

$\large \int_{-1}^{1} \int_{0}^{\sqrt{1-x^{2}}} x^{2}+y^{2}dydx$

![[polar-coord-ex4.png]]

$\Large \int_{0}^{\pi} \int_{0}^{1} r^{2}r dr d \theta$


### Example 2

Find the <u>area</u> of the region bounded above by

$\large y=x$

and below by the circle:

$\large x^{2}+y^{2} -2y =0$

Remember that the generic circle is:

$\large (x-a)^{2} + (y-b)^{2} = r^{2}$

Where (a,b) is the center of the circle. 

So we have to complete the square to figure out how this circle will look.

$\large x^{2} +y^{2} -2y +1 = 1$

so

$\large x^{2} +(y-1)^{2}= 1^{2}$

![[polar-ex-5.png]]

We are looking for the area of the little sliver below $\large y=x$

Now we start converting everything to polar coordinates

1. $\large x^{2} + y^{2} -2y =0$ becomes
   $\large r^{2} -2r\sin \theta = 0 \rightarrow r = 2\sin \theta$

2. $\large y=x$ becomes
   $\large r\sin \theta = r\cos \theta \rightarrow \sin \theta = \cos \theta$
   $\large \tan \theta = 1$
   $\large \theta = \frac{\pi}{4}$
	Basically just saying that $y=x$ is just a 45 deg line


$\Large \int\int_{D^{*}}r dr d \theta$

$\Large \int_{0}^{\frac{\pi}{4}}\int_{0}^{2sin \theta} r dr \text{ }d \theta$

Now we just solve the double integral as normal


### Example 3

Set up the integral for finding th area of the region inside the cardiod
$\large r = 1+\cos \theta$
and outside the circle:
$\large r= 1$

![[cardioid-ex.png]]


$\Large \int\int_{D^{*}}r dr d \theta$

$\Large \int_{- \frac{\pi}{2}}^{\frac{\pi}{2}}\int_{1}^{1+\cos \theta}r \text{ } dr \text{ } d \theta$

$\Large =2\int_{0}^{\frac{\pi}{2}} \int_{1}^{1+\cos \theta} r \text{ } dr  \text{ } d \theta$


### Example 4

Find the <u>area</u> of the [[Lemniscate|lemniscate]]  $\large r^{2} = 4 \cos 2 \theta$

Notice that we want it in the form

$\large r = f(\theta)$

so

$\large r = 2\sqrt{\cos 2  \theta}$

![[lemniscate.png]]

Notice that each petal are sandwiched between the lines

$\large y=x$
and
$\large y = -x$

$\large A = \int \int_{R}r dr d \theta$

To integrate this it will be easiest to take advantage of the symmetry of this shape.

We can take the area of the shape in one quadrant and quadruple it.

$\Large 4 \int_{0}^{\frac{\pi}{4}} \int_{0}^{2\sqrt{\cos 2 \theta}}r \text{ }dr \text{ }d \theta$

$\large = 2 \int_{0}^{\frac{\pi}{4}} 4 \cos(2 \theta) d \theta$

$\large = 4 \sin(2 \theta) \Big|_{0}^{\frac{\pi}{4}}$

$\large = 4$


### Example 5

Show that

$\Large \int_{-\infty}^{\infty} e^{-x^{2}} dx = \sqrt{\pi}$

This integral is the Normal / Gaussian Distribution

Let the integral be $\large I$

Then

$\large I^{2} = \int_{-\infty}^{\infty}\int_{-\infty}^{\infty} e^{-x^{2}-y^{2}}dx dy$

$\large = \int_{-\infty}^{\infty}\int_{-\infty}^{\infty} e^{-(x^{2}+y^{2})}dx dy$

Now we can switch this integral to polar form

$\large \int_{0}^{2\pi}\int_{0}^{\infty}r e^{-r^{2}}drd \theta$ 

Now this is in a form where we can use u substitution

$\large = - \frac{1}{2} \int_{0}^{2 \pi} e^{-r^{2}} \Big|_{0}^{\infty} d \theta$

$\large = \frac{1}{2} \int_{0}^{2 \pi} 1 d \theta$

$\large = \pi$

So 

$\large I = \sqrt{\pi}$


