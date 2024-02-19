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


