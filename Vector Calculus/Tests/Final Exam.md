==ALWAYS CHECK TYPE OF ANSWER (scalar vs vector)==

# Basics

#### [[Quotient Rule]]
#### u-sub
#### [[Vector Calculus/Derivative Rules/Multiplication Rule|Multiplication Rule]]
#### 


# 4 from Unit 1 ([[Vector Calculus/Tests/Test 1|Test 1]]) 

==Check formulas==
### [[Lagrange Multipliers]] ??

### Equation of Plane
- Find [[Normal Vector]] and set the cross of that and smth to 0


# 4 from Unit 2 ([[Test 2]])

Don't need to memorize coordinate transformations

# 4 from Unit 3 ([[Test 3]])

WILL HAVE DIV / CURL
### [[Divergence]] and [[Curl]]
- Could be an actual function or a generic function
- Formulas given
- May be helpful to write derivatives in $\large F_{x}$ form

### [[Scalar Potential]]


# Practice Final

### 2

$$\large \text{velocity} = \vec{F}(t)$$
$$\large \text{acc} = \vec{F}'(t)$$
$$\large \text{pos} = \int\vec{F}(t) \; dt$$

### Example

Find and classify the local extrema of
$$\large f(x,y) = (y-2)x^{2} - y^{2}$$
First we need to find the [[Stationary Points]]
where 
$\large \nabla f = \vec{0}$

$\large \nabla f = \big\langle 2(y-2)x, x^{2} - 2y \big\rangle = \vec{0}$

This gives the system of equations:
$\large 2(y-2)x = 0$
$\large x^{2}-2y = 0 \Rightarrow x^{2} = 2y$
so
$\large x^{3} -4x = 0 \Rightarrow x = 0$

(0,0)
(2,2)
(-2, 2)

Finally to classify these extreme values, we discriminate with the [[The Second Partials Test]]

$\large f_{xx} = 2(y-2)$
$\large f_{yy} = -2$
$\large f_{xy} = 2x$

$$\large D(x,y) = -4(y-2) - 4x^2$$
D(0,0) = 8
so (0,0) is a maximum

D(2,2) = -8
so (2,2) is a saddle point

D(-2,2) = -8
so (-2,2) is a saddle point
