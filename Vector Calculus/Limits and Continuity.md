**==14.2==**

# In 1d
$\Large \lim_{x\to c} =L$  

For every $\large\epsilon \gt 0$ there exists a $\large \delta \gt 0$ such that if $\large|x-c| \lt \delta$ then $\large|f(x) - L| \lt \epsilon$ 
This gives us an interval of $+- \delta$
# In 2d
$\Large \lim_{(x,y)\to(c,d)} f(x,y) = L$

For every $\large\epsilon\gt 0$ there exists a $\large\delta\gt 0$ such  that if $\large0\lt \sqrt{(x-c)^{2}+(y-d)^{2}}\lt \delta$
This equation gives us a circle of radius $\delta$
- This can also be expanded for any number of variables creating spheres, hyper spheres, etc.

### Generalization of open/closed interval

Open or closed circle, sphere, hyper sphere, etc

##### Notation for an open circle
$\Large D((a,b),r) = \{(x,y):\sqrt{(x-c)^{2}+(y-d)^{2}} \lt r\}$ 

Drawn with dashed lines
The set of all point $\large(x,y)$ where the inequality holds

##### Notation for a closed circle
$\Large \bar{D((a,b),r)} = \{(x,y):\sqrt{(x-c)^{2}+(y-d)^{2}} \le r\}$

Drawn with solid line

#### Notation for some 2d shape

A point $\large P_{0}= (x_{0},y_{0})$ is an interior point of S (not on the boundary) if we can draw some open/closed circle, centered at $\large P_{0}$ with a positive radius and the entirety of the circle lies within S.

A point $\large P_{0}$ is a boundary point of S if every disk centered at $\large P_{0}$ contains points inside of S and outside of S

The set of all boundary points is called the boundary of S and is denoted by  $\large \delta A$ 

# Properties of Limits

Suppose that $\large \lim_{(x,y)\to (c,d)} f(x,y) = L$ and $\large \lim_{(x,y)\to (c,d)}g(x,y) = M$
Then:
1. $$\large\lim_{(x,y)\to(c,d)} [f(x,y) + g(x,y)] = L+M$$
2. $$\large \lim_{(x,y)\to (c,d)} Af(x,y) = AL$$
	- We can factor out constants
3. $$\large\lim_{(x,y)\to(c,d)} [f(x,y)*g(x,y)] = L*M$$
4. $$\large\lim_{(x,y)\to(c,d)} \frac{f(x,y)}{g(x,y)} = \frac{L}{M} \text{ provided } M\ne 0$$
5. $$\large\lim_{(x,y)\to(c,d)} [f(x,y)]^{n} = L^{n}$$

### When Limits Don't Exist (DNE)

In 1d space there are only 2 ways to approach a point, but in 2d space we can approach a point from an infinite number of angles

What exactly does it mean if
$\large \lim_{(x,y)\to (c,d)} f(x,y)$  DNE?

In order to show that $\large \lim_{(x,y)\to (c,d)} f(x,y)$  DNE we will use the [[Two Path Test]]