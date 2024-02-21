==**15.2**==

How would we set up the limits of integration over a triangle?

$\large \int \int_{R} f(x,y)dA = \text{ ?}$

# Types of Regions

### Vertically Simple Region

A vertically simple region is a region $\large D$ is a region of the form $\large D = \{(x,y): a\le x\le b, g_{1}(x) \le y\le g_{2}(x)\}$

Two boundaries of our region are represented by vertical lines.
##### Example:
![[vertically-simple-region.png]]

In this case:

$\large g_{1}(x) = x^{3}$
and
$\large g_{2}(x) = 1+x^{3}$

==In this case always use the order of integration== $\large dy \text{ } dx$

### Horizontally Simple Region

A horizontally simple region is a region $\large D$ in the form $\large D=\{(x,y): h_{1}(y)\le x\le h_{2}(y), c\le y\le d\}$

Two boundaries of the region are defined by  horizontal lines

![[horizontally-simple-region.png]]

==In this case, always use the order of integration== $\large dx \text{ } dy$

### Both Vertically and Horizontally Simple

Think of a triangle. This is both cases

### Neither Vertically or Horizontally Simple

# Examples

##### Vertically Simple Region
Evaluate $\large \int_{3}^{5}\int_{-x}^{x^{2}} 4x +10y dydx$

Since the region of integration is a function of $\large x$, we know that this is vertically simple.

![[vertically-simple-ex.png]]

Now that we've determined that this is a vertically simple region and know to integrate in the order $\large dy \text{ }dx$ we just solve the integral.


##### Horizontally Simple Region

Evaluate $\large \int_{0}^{1}\int_{0}^{y^{2}}2ye^{x}dxdy$

![[horizontally-simple-ex.png]]

Notice that this shape is technically both horizontally and vertically simple, but we will treat it as a horizontally simple shape since the bounds are given in terms of $\large y$.

We just solve this in the order $\large dx \text{ } dy$


# How to find area of a random shape

$\large \int_{a}^{b} 1dx =$ length of $\large [a,b]$

so

$\large \int \int_{D} 1dA =$  area of D

and

$\large \int \int\int_{D}1dV =$ volume of D

# Examples

$\large D$ is the region bounded by $\large y=x^{2}-2$ and $\large y=x$ 
Find the area of D

![[area-of-some-region-ex.png]]

This region is either vertically simple.

To get the vertically boundaries we need to solve

$\large x^{2}-2 =x$

This gives $\large x = 2, x=-1$ for the boundaries

so we solve the integral

$\large \int_{-1}^{2}\int_{x^{2}-2}^{x}1dydx = \int_{-1}^{2} x-(x^{2}-2)dx$

If we instead choose to set up the integral as a horizontally simple region we will need to use two double integrals.

We will measure the area above and below a horizontal line at -1 and add the two integrals.

Since were flipping directions we need to solve the equations for $\large y$

$\large y = x^{2} -2 \Leftrightarrow x = \sqrt{y+2}$

$\large  y = x \Leftrightarrow x = y$

This gives the two double integrals:

$\large \int_{-2}^{-1} \int_{\sqrt{y+2}}^{-\sqrt{y+2}}1dx \text{ }dy$

and

$\large \int_{-1}^{2}\int_{y}^{\sqrt{y+2}} 1 dx \text{ }dy$

# Sometimes you must pick a particular order

Evaluate $\large \int_{0}^{4}\int_{\frac{x}{2}}^{2}e^{y^{2}}dydx$

Notice that $\large e^{y^{2}}$ doesn't have an anti-derivative.

This means we <u>HAVE</u> to switch the order of integration

![[example-double-integral-need-to-swtich.png]]

To switch this integration we need to write it in a way that works for $\large y$

$\large y =\frac{x}{2} \Leftrightarrow x = 2y$

So:

$\large \int_{0}^{2}\int_{0}^{2y}e^{y^{2}}dx dy$

$\large = \int_{0}^{2}(2ye^{y^{2}} -0)$

Now its in a form where u-substitution will work and we get $\large e^{4}-1$

### Finding Volume

Find the volume of the pyramid bounded by the coordinate planes (the x-y, x-z, and y-z plane) and $\large 3x +6y +4z -12=0$

![[coordinate-plane-pyramid.png]]

$\large V = \int \int_{R} f(x,y) dA$

To get our $\large f(x,y)$ solve the 4th plane for $\large z$

$\large f(x,y) =  \frac{3}{4}(4-x-2y) = z$

Notice that one of our bounds of integration is a line on the x-y coordinate plane.

To find this we need to solve for $\large f(x,y) = 0$

x-intercept $\large = (4,0,0)$

y-intercept $\large= (0,2,0)$

Now we just find the equation of the straight line that passes through this point.

![[pyramid-ex-2.png]]

The equation of this line is 
$\large x+2y -12 = 0$
$\large \Leftrightarrow y = -\frac{1}{2}x+2$
$\large \Leftrightarrow x= 4-2y$

Using this equation we can set up the region of integration.

![[pyramid-ex-3.png]]

So

$\large V = \int_{0}^{4}\int_{0}^{2- \frac{x}{2}}f(x,y)dydx$

or

$\large V = \int_{0}^{2}\int_{0}^{4-2y}f(x,y)dxdy$

