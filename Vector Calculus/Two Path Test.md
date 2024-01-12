Test to show if a 2d limit DNE

We have to come up with two different approaches to the same point that lead to different answers. Finding two answers immediately shows that the limit does not exist.

### Ex.
Show that $\large\lim_{(x,y)\to(0,0)}\frac{x^{2}-y^{2}}{x^{2}+y^{2}}$ does not exist (DNE)

**Approach 1:**
First, approach (0,0) along the x axis (y=0)
Then, $\large f(x, y)\to f(x,0)= \frac{x^{2}}{x^{2}}=1$

**Approach 2:**
Next, approach (0,0) along the y axis (x=0)
Then, $\large f(x,y)\to f(0,y)=\frac{-y^{2}}{y^{2}} = -1$

Since $1\ne -1$, the limit DNE by the two path test

### Ex.
Find $\large\lim_{(x,y)\to(0,0)}\frac{xy}{x^{2}+y^{2}}$ if it exists

First, approach (0,0) along the x-axis
Then, $\large f(x,y) \to f(x,0) = \frac{0}{x^{2}} = 0$

Notice that if we approached from the y axis we would also get 0

Instead we will approach (0,0) along the line $\large y=x$
Then, $\large f(x,y)\to f(x,x)=\frac{x^{2}}{2x^{2}}=\frac{1}{2}$
This shows that the limit does not exist

### Ex.
Find $\large \lim_{(x,y)\to(0,0)}\frac{xy^{2}}{x^{2}+y^{4}}$ if it exists

First, approach (0,0) along the line $\large y=2x$
Then, $\large f(x,y)\to f(x,2x) = \frac{x(2x)^{2}}{x^{2}+(2x)^{4}} = \frac{4x^{3}}{x^{2}+16x^{4}} =\frac{4x}{1+16x^{2}}$ this function approaches 0

Next, approach (0,0) along the parabola $x=y^{2}$
Then, $\large f(x,y)\to f(y^{2},y) = \frac{y^{4}}{y^{4}+y^{4}} = \frac{1}{2}$

### Ex.
Find $\large \lim_{(x,y)\to (0,0)} \frac{x^{2}-xy}{\sqrt{x}-\sqrt{y}}$ if it exists
Since it is $\frac{0}{0}$ it may not exist

Multiply by conjugate

$\large = \lim_{(x,y)\to (0,0)} \frac{x^{2}-xy}{\sqrt{x}-\sqrt{y}} * \frac{\sqrt{x}+\sqrt{y}}{\sqrt{x}+\sqrt{y}}$
$\large = \lim_{(x,y)\to (0,0)} \frac{(x^{2}-xy)(\sqrt{x}+\sqrt{y})}{x-y}$
$\large = \lim_{(x,y)\to (0,0)} x(\sqrt{x}+\sqrt{y})$
