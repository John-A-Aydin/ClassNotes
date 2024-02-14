==**15.1**==

# Notation

A rectangle $\large R$ can be written as:

$\large R = [a,b]\times[c,d] = \{(x,y): a\le x\le b \land c\le y\le d\}$

# Evaluating a Double Integral Over a Rectangle

$\large \int \int_{R} f(x,y) dA = \int \int f(x,y) dxdy = \int \int f(x,y) dydx$

Notice that 

$\large [a,b]$ corresponds to our $\large x$ values (bounds of integration for $\large dx$)

and

$\large [c,d]$ corresponds to our $\large y$ values (bounds of integration for $\large dy$)

so

$\large \int_{a}^{b} \left(\int_{c}^{d} f(x,y) dy\right)dx = \int_{c}^{d} \left( \int_{a}^{b} f(x,y) dx\right)dy$

1. Integrate with the innermost variable first, treating the other variables as constants.
2. Integrate with respect to the outermost variable as normal.

### Fubin's Theorem

If $\large f(x,y)$ is continuous on the rectangle

$\large R = [a,b]\times[c,d] = \{(x,y): a\le x\le b \land c\le y\le d\}$

then $\large \int \int_{R} f(x,y)dA = \int_{a}^{b}\int_{c}^{d}f(x,y)dydx = \int_{c}^{d}\int_{a}^{b}f(x,y)dxdy$

# Geometric Interpretation

$\large \int \int_{R} f(x,y) dA$

represents the volume of an object whose top is the surface $\large z = f(x,y)$ and base is the region R.

![[double-integral-over-rectangle.png]]



### Example

Find the volume of the solid under the surface $\large z = 4-x^{2}-y$  over $\large R = [0,1]\times[0,2]$

$\large V = \int\int_{R}f(x,y)dA$

$\large = \int_{0}^{2}\int_{0}^{1}4-x^{2}-y dxdy$

$\large = \int_{0}^{2}\left[4x -\frac{1}{3}x^{3}-yx\right]_{0}^{1}$

$\large =\int_{0}^{2} \frac{11}{3}-y dy$

$\large = \left[\frac{11}{3} - \frac{1}{2}y^{2}\right]_{0}^{2}$

$\large = \frac{16}{3}$

### Example Where Order of Integration Matters

Find $\large \int \int_{R} xcos(xy) dA$ over $\large R=[0, \frac{\pi}{2}]\times [0,1]$

Notice that if we do it as $\large \int \int f(x,y)dxdy$, we have to compute it with integration by parts, but if we do it as $\large \int \int f(x,y)dydx$,  the integral is very straight forward.

**Moral of the story:** Always look at both orders especially if the integral looks kinda hard.