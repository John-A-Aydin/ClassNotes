==**16**==

Generalization of
$$\large \int_{a}^{b} f(x) \; d x$$
Think of $\large [a, b]$  as a path $\large C$ from $\large x=a$  to $\large x=b$

Now, let $\large C$ be any 2d (planar) curve given by
$\large \vec{r}(t) = \langle x(t), y(t) \rangle$

$\large C$ starts at $\large ( x(a) , y(a) )$  and stops at $\large ( x(b) , y(b) )$
How do we integrate a function $\large f(x,y)$ along $\large C$?

##### Notation:
$$\large \int_{C} f(x,y) \; d S$$
where $\large dS$ represents the [[Arc Length|arc length]].
![[Line or Path Integral.png]]

This is the area of a surface whose shape is defined by the path under $\large f(x,y)$ defined by $\large C$

The overall idea of the integral is splitting this path into small partitions $\large dS$
These partitions have two components:
$\large dx$: The change in x from one side to the other
$\large dy$: The change in y from one side to the other

$\large dS$, $\large dx \text{ , } dy$ form a right triangle so:
$\large dS = \sqrt{(dx)^{2}+(dy)^{2}}$

$\large f(x,y) \Rightarrow f(x(t), y(t))$
$\large dS = \sqrt{(\frac{dx}{dt})^{2} + (\frac{dy}{dt})^{2}}\;dt \Rightarrow dS = ||\vec{r}'(t)||dt$


$$\Large \int_{C} f(x,y) \; d S = \int_{a}^{b} f(x(t), y(t)) \; \sqrt{[x'(t)]^{2} + [y'(t)]^{2}}\; dt$$

### Properties of Line Integrals
Let $\large a \text{ and } b$ be constants
$$\large \int_{C} af(x,y) \pm bg(x,y) \; d S  = a\int_{C} f(x,y) \; d S \pm b \int_{C} g(x,y) \; d S \tag{1}$$
Let $\large -C$ be $\large C$, but traversed in the opposite direction.
$$\large \int_{-C} f(x,y) \; d S = - \int_{C} f(x,y) \; d S \tag{2}$$
Let $\large C$ be a curve that is composed of several components $\large C_{1} \text{, } C_{2}\text{, }C_{3}\text{ ... } C_{n}$ 
$$\large \int_{C} f(x,y) \; d S = \sum\limits_{1}^{n}\int_{C_{n}} f(x,y) \; d S \tag{3}$$




### Example 1

Evaluate
$$\large \int_{C} x^{2}y \; d S$$
where $\large C$ is given by
$\large x(t) = 3 \cos(t)$
$\large y(t) = 3 \sin(t)$
$\large 0 \le t \le \frac{\pi}{2}$

$$\large \int_{C} f(x,y) \; d S = \int_{0}^{\frac{\pi}{2}} 81 \cos^{2}(t)\sin(t) \; d t = 27$$


### Example 2

Suppose that the force acting upon a particle at a given point $\large ( x , y , z )$ is given by the [[Vector Fields]]
$$\large \vec{F}(x,y,z) = \langle M(x,y,z), N(x,y,z), P(x,y,z) \rangle$$
We wish to calculate the work done by $\large \vec{F}(x,y,z)$ to move the particle along a given path $\large C$

Let $\large \vec{r}(t) = \langle x(t), y(t), z(t) \rangle$ be the position of a point $\large Q$ on the curve $\large C$. Recall l that $\large \vec{T}$ is the [[Unit Tangent Vector of VVF|unit tangent vector]]. The work done by $\large \vec{F}$ to move $\large Q$ a start distance $\large \Delta S$ along $\large C$ is
$$\large \Delta W = \vec{F}(\vec{T}\Delta S) = \text{(force)(distance)}$$
so in total, to move from the starting point of $\large C$ to the stopping point of $\large C$ we get
$$\large W = \int_{C}\vec{F} \vec{T} \; d S \tag{0}$$
This can be simplified to
$$\large W = \int_{C}\vec{F} \;d \vec{r}\tag{1}$$
where 
$\large d \vec{r} = \langle dx, dy, dz \rangle \; dt$
Since $\large \vec{F}  = \langle M, N, P \rangle$, we also have
$$\large W = \int_{C} M\;dx +  N \; dy + P \; dz \tag{2}$$

#### Example

Let 
$\large \vec{F}(x,y,z) = \langle y-x^{2}, z-y^{2}, x-z^{2} \rangle$
and
$\large \vec{r}(t) = \langle t, t^{2}, t^{3} \rangle$

Find
$\large W = \int_{C} \vec{F} \cdot d \vec{r}$

first we need to find
$\large \vec{F}(\vec{r}(t)) = \langle 0, t^{3} - t^{4},t-t^{6} \rangle$
Next,
$\large d \vec{r} = \langle1,2t,3t^{2} \rangle \; dt$
So
$\large \vec{F}\cdot d \vec{r} =[2t^{4}- 2t^{5} + 3t^{3}-3t^{8}]dt$
Finally
$$\large \int_{C} \vec{F} \; d \vec{r} = \int_{0}^{1} [2t^{4} - 2t^{5} + 3t^{3} - 3t^{8}] \; d t = \frac{29}{60}$$

### Example 3

Evaluate 
$$\large \int_{C} xy^{2} \; d x + xy^{2}dy$$
where $\large C = C_{1} \cup C_{2}$ 
and $\large C_{1}$ is given by the two points $\large ( 0 , 2 )$ and $\large ( 3 , 2 )$
and $\large C_{2}$ is given by the two points $\large ( 3,2   )$ and $\large ( 3,5  )$

Using (3), this integral can be split by $\large C_{1}$ and $\large C_{2}$.

$$\large \int_{C_{1}} xy^{2} \; d x + xy^{2} \; dy$$
On $\large  C_{1} \text{, } y=2 \text{ so } dy = 0$
This makes the integral over $\large C_{1}$
$$\large \int_{0}^{3} 4x \; d x = 18$$
$$\large \int_{C_{2}} xy^{2} \; d x + xy^{2} \; dy$$
On $\large C_{2} \text{, } x=3 \text{ so } dx = 0$
This makes the integral over $\large C_{2}$
$$\large \int_{2}^{5} 3y^{2} \; d y = 117$$
so 
$$\large \int_{C} xy^{2} \; d x + xy^{2} \;dy = 135$$

Let $\large C_{3}$ be the line that is the hypotenuse to the triangle formed by $\large C_{1} \text{ and } C_{2}$
On $\large C_{3} \text{, } y= x+2$ and $\large dy = dx$ so
$$\large \int_{C_{3}} xy^{2} \; d x + xy^{2} \;dy = 2\int_{0}^{3} x(x+2)^{2} \; d x = \frac{297}{2}$$
This tells us that it is harder to push a particle along $\large C_{3} \text{ than } C$, subject to the vector field 

#### Note
If $\large C$ is a closed curve, then you will frequently see
$$\large \oint_{C}\vec{F}\cdot d \vec{r}$$

### Example 4: Path Independence

Line integrals where this happens are said to be <u>independent of path</u> or <u>path independent</u>
When do we have path independence?

If $\large \vec{F}$ satisfies $\large \nabla f = \vec{F}$, we can use the [[The Fundamental Theorem of Line Integrals]]

##### Example
Suppose that $\large \vec{F}$ is the gradient of
$$\large f(x,y,z) = \frac{-1}{x^{2}+y^{2}+z^{2}}$$
Compute the work done by $\large \vec{F}$ to move a particle along any curve joining $\large ( 1 , 0 ,  0)$ and $\large ( 0 , 0 , 2 )$.
Recall:
$$\large W = \int_{C} \vec{F} \cdot \vec{r} = \int_{C} \nabla f \cdot d \vec{r} = f(0,0,2) - f(1,0,0) = \frac{3}{4}$$
by the [[The Fundamental Theorem of Line Integrals|fundamental theorem of line integrals]]

### When do we have path independence

A vector field $\large \vec{F}$ is <u>conservative</u> if
$$\large \vec{F} = \nabla f$$
for some scalar function $\large f$, called the <u>scalar potential</u> of $\large \vec{F}$

$\Large \int_{C} \vec{F} \cdot d \vec{r}$ 
is independent of path iff $\large \vec{F}$ is conservative

#### How can we tell if $\large \vec{F}$ is conservative

#### 1. The Cross Partials Test
Let $\large \vec{F}(x,y) = \langle M(x,y), N(x,y) \rangle$
Then $\large \vec{F}$ is conservative iff
$$\large \frac{\partial M}{\partial y} = \frac{\partial N}{\partial x}$$

