==**14.8**==
#VecTest1

Technique for solving ==constrained== optimization problems (finding [[Extrema|extrema]]).
- maximize or minimize $\large f(x,y)$ subject to $\large g(x,y) = C$
- $\large f(x,y)$ is called the "objective function"
- $\large g(x,y) = C$  is called the "constraint"

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

Note that since x,y,z are dimensions they must all be positive

We know that $\large \nabla C(x,y,z) = \lambda \nabla V(x,y,z)$

So we get the system of equations:

(1) $\large 3y +2z = \lambda yz$

(2)  $\large 3x+2z = \lambda xz$

(3)  $\large 2x+2y = \lambda xy$

(4)  $\large xyz = 12$

Notice that in (1), (2), and (3) it is really easy to solve for lambda
Also, since x,y,z are not 0 we don't have to worry about dividing by 0

(5)  $\large \lambda = \frac{3}{z} + \frac{2}{y}$

(6)  $\large \lambda = \frac{3}{z}+ \frac{2}{x}$

(7)  $\large \lambda = \frac{2}{y} + \frac{2}{x}$

so using (5) and (6)

$\large \frac{3}{z} + \frac{2}{y} = \frac{3}{z} \frac{+2}{x} \Rightarrow x=y$

and using (5) and (7)

$\large \frac{3}{z} + \frac{2}{y} = \frac{2}{y} + \frac{2}{x} \Rightarrow z = \frac{3}{2}x$

Now we just use (4)

$\large x = 2$

$\large y = 2$

$\large z = 3$

There is only one solution and this technically could be a maximum or minimum but because of the phrasing of the question we know it is a minimum

To find the min cost we just evaluate at the solution

$\large C(2,2,3) = 36$

### Example

Find the absolute extrema of
$\large f(x,y) = 4x + 6y +5$

on the set $\large S = \{(x,y): x^{2}+3y^{2} = 28\}$
(the set of all points (x,y) such that the equation holds)

This time the constraint is given in set notation, but it means the same thing.

(1)  $\large 4 = \lambda 2x\Rightarrow 2 = \lambda x \Rightarrow x = \frac{2}{\lambda}$
(2)  $\large 6 = \lambda 6y\Rightarrow 1 = \lambda y\Rightarrow y = \frac{1}{\lambda}$
(3)  $\large x^{2} + 3y^{2} = 28$

Note that lambda is not inherent to the problem so we can impose any restrictions we want on it. For this problem we will say that $\large \lambda \ne 0$ 

$\large \frac{2}{\lambda}^{2} + 3(\frac{1}{\lambda})^{2} = 28 \Rightarrow \lambda = \pm \frac{1}{2}$

For $\large \lambda = \frac{1}{2}$,
$\large (4,2)$

For $\large \lambda = \frac{-1}{2}$
$\large (-4, -2)$

Now to find out which one is the max/min we just plug them in to the original function.

$\large f(4,2) = 33$

$\large f(-4,-2) = -23$

So $\large (4,2)$ is the absolute max and $\large (-4,-2)$ is the absolute min

