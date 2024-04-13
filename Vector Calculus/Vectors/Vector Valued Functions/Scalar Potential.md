A vector field $\large \vec{F}$ is <u>conservative</u> if
$$\large \vec{F} = \nabla f$$
for some scalar function $\large f$, called the <u>scalar potential</u> of $\large \vec{F}$

### Example **==TEST 3==**

Let $\large \vec{F}(x,y) = \langle 4x^{3} + 9x^{2}y^{2}, 6x^{3}y + 6y^{5} \rangle = \langle M(x,y), N(x,y) \rangle$

First we verify that $\large \vec{F}$ is conservative

$$\large \frac{\partial M}{\partial y} = 18x^{2}y = \frac{\partial N}{\partial x}$$
Now we find the scalar potential
$$\large M(x,y) = \frac{\partial f}{\partial x} \text{ and } N(x,y) = \frac{\partial f}{\partial y}$$
If we integrate both sides we can find $\large f$
$$\large \int \frac{\partial f}{\partial x} \;dx = \int4x^{3}+ 9x^{2}y^{2} \; dx \Rightarrow f(x,y) = x^{4}+3x^{3}y^{2} + g(y)$$
To get rid of the hanging function of $\large y$, we must calculate the integral of $\large y$.
$$\large \frac{\partial f}{\partial y} = 6x^{3}y + g'(y) = 6x^{3}y + 6x^{5} \Rightarrow g(y) = y^{6}+C$$
Therefore
$$\large f(x,y) = x^{4} + 4x^{3}+y^{2} +y^{6} + C$$
is the scalar potential of $\large \vec{F}$