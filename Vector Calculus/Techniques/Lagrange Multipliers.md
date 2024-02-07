==**14.8**==

Technique for solving constrained optimization problems (finding [[Extrema|extrema]].
- maximize or minimize $\large f(x,y)$ subject to $\large g(x,y) = C$
- $\large f(x,y)$ is called the "objective function"
- $\large g(x,y) + C$  is called the "constraint"

Notice that the constraint is a [[Level Curve|level curve]]

The solutions to this problem can be found by solving the system of equations:

$\large \nabla f(x,y) = \lambda \nabla g(x,y)$

$\large g(x,y) = C$

for x, y and (maybe) $\large \lambda$ which is the Lagrange multiplier

Notice that since $\large \nabla f$ and $\large \nabla g$ are vectors we essentially have 3 equations

### Example

Find the absolute extrema of $\large f(x,y) = x^{3}y$  subject to $\large x^{2}+3y^{2} = 48$

We need to find x,y, $\lambda$ so that the aforementioned system of equations holds

##### Finding the system of equations

$\large \nabla f = \langle 3x^{2}y, x^{3}\rangle$
and
$\large \nabla g = \langle 2x, 6y \rangle$

so our system of equations is

$\large 3x^{2}y = \lambda 2x$

$\large x^{3} = \lambda 6y$

$\large x^{2} +3y^{2} = 48$

##### Solving the system of equations

We can start with equation 1

$\large 3x^{2}y-\lambda 2x = 0$
$\large 3xy - 2\lambda = 0$
so
$\large x=0 \text{ or } 3xy = 2\lambda$

use these initial values by plugging them in to other equations and looking for "lies"

The solutions to this in the form $\large (x,y)$ are
$\large (0,4)$
$\large (0,-4)$
$\large (6,2)$
$\large (6, -2)$
$\large (-6, 2)$
$\large (-6, -2)$

Remember that we don't have to find lambda

Finally we plug all of these values into $\large f$ and compare the results

$\large f(0, 4) = 0$
$\large f(0, -4) = 0$
...

We will find that the absolute maximums in the form $\large (x,y,z)$ are
$\large (6,2, 432)$ and $\large (-6, -2, 432)$

The absolute minimum points in the form $\large (x,y,z)$ are
$\large (-6, 2, -432)$ and $\large (6,-2, -432)$


### Example

An open top box has a fixed volume of 12 $m^{3}$ 
The material for the bottom costs $3 per sq meter and the sides cost $1 per square meter.

What dimensions minimize the cost per $m^{3}$?

Note that the cost is dependent on x, y, and z

The cost can be defined as:
$\large C(x,y,z) = 3xy + 2xz + 2yz$

And the constraint is:
$\large V(x,y,z) = xyz = 12$
