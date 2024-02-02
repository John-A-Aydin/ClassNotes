==**14.7**==

# Absolute Extrema

### Definition

Let $\large P_{0}$ be a point in the domain of $\large f$ 

Then $\large f(P_{0})$  is an absolute max value of $\large f$ if

$\large \forall P\in \text{domain of }f(f(P_{0}) \ge f(P))$

And $\large f(P_{0})$ is an absolute min value of $\large f$ if

$\large \forall P\in \text{domain of }f(f(P_{0}) \le f(P))$




# Local Extrema

For local extrema we use the same inequalities as the absolute extrema but they only need to hold for all points $\large P\in D(P_{0}, r)$ for some $r>0$.

Note that $\large D(P_{0}, r)$ represents a circle, sphere, etc of radius r centered around $\large P_{0}$

### Theorem
If $\large f$ is continuous on a closed, bounded set $\large S$, then $\large f$ attains both an absolute maximum and an absolute min on $\large S$

There are 3 possibilities for the locations of these extrema
1. Points where all of the derivatives equal 0 (Stationary Points) (flat tangent plane at this point)
2. Points on the edges of the interval
3. Points where one of the derivatives are undefined (Singular Points)



### Example

Find the local extrema of $\large f(x,y) = x^{2}-2x +\frac{y^{2}}{4}$ 

(1) Since no $\large S$ is given there are not boundary points

(2) The derivatives are not undefined at any points (No singular points) 

(3) Now we have to find the stationary points

$\large \nabla f = \langle 2x-2, \frac{y}{2}\rangle = \vec{0}$

so 

$\large 2x-2  = 0$  and $\large \frac{y}{2} = 0$

so there is a local extrema at $\large (1,0)$

but we don't know if it is a max or min or neither

