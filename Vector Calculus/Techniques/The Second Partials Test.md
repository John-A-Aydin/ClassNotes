==**14.7**==
#VecTest1 
A test to find [[Extrema|extrema]] using the [[Gradient|gradient]]

Suppose that $\large f$ has continuous 2nd derivatives and that $\large P_{0}$ satisfies $\large \nabla f(P_{0}) = \vec{0}$

Define $\large D(x,y) = f_{xx}(x,y)f_{yy}(x,y) - f^{2}_{xy}(x,y)$ 
as the [[Vector Calculus/Discriminate|discriminate]] of $\large f(x,y)$

1. If $\large D(P_{0})$ is positive and $\large f_{xx}(P_{0})$ or $\large f_{yy}(P_{0})$ is negative then $P_{0}$ is a local maximum with\ max value $\large = f(P_{0})$
2. If $\large D(P_{0})$ is positive and $\large f_{xx}(P_{0})$ or $\large f_{yy}(P_{0})$ are positive then $\large P_{0}$ is a local minimum with min value $\large = f(P_{0})$
3. If $\large D(P_0)$ is negative then $P_{0}$ is a [[Saddle Point|saddle point]]
4. If $\large D(P_{0}) = 0$ then the test is inconclusive

### Example

Find the local extreme value of
$\large f(x,y) = 3x^{3} +y^{2} -9x +4y$

###### 1st
Find the stationary points
$\large \nabla f = \langle 9x^{2} -9, 2y+4\rangle =\vec{0} = \langle0,0\rangle$
so
$\large x \pm 1$  and $\large y = -2$
###### 2nd
Discriminate

$\large f_{xx} = 18x$
$\large f_{yy}=2$
$\large f_{xy}=0$

$\large D(x,y) = 18x*2-0^{2} = 36x$
###### 3rd
Figure out which case we have

### Example 2

Find the minimum distance between the origin and the surface $\large z^{2} = x^{2}y +4$

This can be rewritten as a [[Level Curve]]
$\large z^{2}-x^{2}y = 4$

Let $\large P$ be any  point on this surface
We want to minimize the distance between $\large P$ and (0,0,0)

$\large d(P, (0,0,0)) = \sqrt{x^{2}+y^{2}+z^{2}}$

Notice that if we minimize the distance squared we are also minimizing the distance

$\large d(P,(0,0,0)) = x^{2}+y^{2}+z^{2} = x^{2} + y^{2} +x^{2}y +4 = f(x,y)$

##### 1st
Find the stationary points
$\large \nabla f = \langle 2x + 2xy, 2y + x^{2}\rangle = \vec{0}$

This gives us a nonlinear system of equations:
$\large 2x+2xy = 0$  and $\large 2y +x^{2} = 0$

(0,0) and ($\pm\sqrt{2}$, -1)

##### Repeat steps from prev example
