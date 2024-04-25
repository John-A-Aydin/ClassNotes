==**12**== 
#TODO sort
### Definition
Let $\large \vec{u} = \langle u_{1}, u_{2}, u_{3}\rangle$ and $\large \vec{v} = \langle v_{1},v_{2}, v_{3}\rangle$

Then $\large \vec{u} \times \vec{v}$ is given by the [[Determinant|determinant]] of the following matrix
$$\large \begin{bmatrix} \hat{i}  & \hat{j} & \hat{k}  \\ u_{1} & u_{2} & u_{3}  \\ v_{1} & v_{2} &v_{3}  \end{bmatrix}$$
This problem can be broken up into smaller determinants

$$\large \text{det}\begin{bmatrix} u_{2} & u_{3}  \\ v_{2} & v_{3}   \end{bmatrix}\hat{i} - \text{det} \begin{bmatrix} u_{1} & u_{3}  \\ v_{1} & v_{3} \end{bmatrix}\hat{j}+ \text{det} \begin{bmatrix} u_{1} & u_{2} \\ v_{1} & v_{2} \end{bmatrix}\hat{k}$$

### Properties

Let $\large s$, $\large t$ be scalars (constants) and $\large u$, $\large v$, and $\large w$ be non-zero vectors.
Then:
1. $$\large (s \vec{v}) \times (t \vec{w}) = (st)(\vec{v}\times \vec{w})$$
2. Cross product distributes over vector addition$$\large \vec{w} \times(\vec{u} +\vec{v}) = \vec{w}\times\vec{u} + \vec{w}\times \vec{v}$$$$\large(\vec{u} +\vec{v}) \times \vec{w} = \vec{u} \times \vec{w }+\vec{v} \times \vec{w}$$
3. $$\large \vec{v}\times \vec{w} = -(\vec{w} \times \vec{v})$$
4. $$\large \vec{v} \times (s \vec{v}) = s(\vec{v} \times \vec{v}) = \vec{0}$$
5. $$\large \vec{0} \times \vec{v} = \vec{v} \times \vec{0} = \vec{0}$$

Looking at the definition of the cross product, computing the determinant clearly shows why $\large \vec{v} \times \vec{v} = \vec{0}$  #TODO 

### Other important properties

1. Given $\large \vec{v} \text{ , } \vec{w} \ne \vec{0}$, $\large \vec{v} \times \vec{w}$ is orthogonal to $\large \vec{v}$ and $\large w$
2. If $\large \vec{v} \text{ , } \vec{w} \ne \vec{0}$ and $\large 0 \le\theta \le \pi$ is the angle between $\large \vec{v} \text{ and } \vec{w}$, then$$\large ||\vec{v} \times \vec{w}|| = ||\vec{v}|| ||\vec{w}|| \sin(\theta)$$
3. As a consequence of 2, we get the following:$$\large \text{Area of parallelogram formed by } \vec{v} \text{ and } \vec{w} = ||\vec{v} \times \vec{w}|| = ||\vec{v}|| ||\vec{w}|| \sin(\theta)$$
4. As a consequence of 3, we get the following:$$\large \text{Area of triangle formed by } \vec{v} \text{ and } \vec{w} = \frac{||\vec{v} \times \vec{w}||}{2} = \frac{||\vec{v}|| ||\vec{w}|| \sin(\theta)}{2}$$

   