==**14.5**==

# Operations on Vectors

Let $\large \vec{v} = \langle v_{1}, v_{2}, \text{ ... } v_{n}\rangle$ and $\large vec{u} = \langle u_{1}, u_{2}, \text{ ... } u_{n} \rangle$ and C be any real number

### Scalar Multiplication
$$\Large C\vec{v} = \langle Cv_{1}, Cv_{2,}\text{ ... }Cv_{n}\rangle$$
- Scalar multiplication stretches the vector
- When C is negative, the vector is reflected over both axes

### Vector Addition
$$\Large \vec{u}+\vec{v} = \langle u_{1}+v_{1}, u_{2}+v_{2}, \text{ ... } u_{n}+v_{n}\rangle$$

### Dot Product (Inner Product)
$$\Large \vec{u}\cdot \vec{v} = u_{1}v_{1}+u_{2}v_{2} \text{ ... } = \sum\limits_{i=1}^{n}u_{i}v_{i}$$
The dot product of two vectors results in a scalar value.

Thanks to the law of cosines we can use the dot product to compute the angle $\large \theta$ between two given vectors.

$\large \vec{u}\cdot \vec{v} = ||\vec{u}||||\vec{v}||cos \theta$ 


# Magnitude

The magnitude / norm of a vector is its length.

$\Large ||\vec{v}|| = \text{ magnitude } = \text{ scalar}$

If $\vec{v} = <v_{1}, v_{2}, \text{ ... }, v_{n}$ then

$\large ||\vec{v}|| = \sqrt{v_{1}^{2} + v_{2}^{2} + \text{ ... } + v_{n}^{2}} = \sqrt{\sum\limits^{n}_{i=1}v^{2}_{i}}$

### Example
$\large \vec{v} = <2,5>$,   $\large ||\vec{v}|| = \sqrt{2^{2}+5^{2}} = \sqrt{29}$

### [[Unit Vector]]

### IDEK

Let $\large \vec{u} = \langle u_{1}, u_{2}, u_{3}\rangle$ and $\large \vec{v} = \langle v_{1},v_{2}, v_{3}\rangle$

Then $\large \vec{u} \times \vec{v}$ is given by the determinant of the following matrix

| i     | j     | k     |
| ----- | ----- | ----- |
| $u_1$ | $u_2$ | $u_3$ |
| $v_1$ | $v_2$ | $v_3$ |

This problem can be broken up into smaller determinants

$\large <mat> \hat{i} - <mat> \hat{j}+ <mat>\hat{k}$ 

#### Theorem

If $\large \vec{u} \text{ and } \vec{v}$ are nonzero vectors that are not multiples of each other, 
then $\large \vec{u} \times \vec{v}$  is orthogonal to both $\large \vec{u} \text{ and } \vec{v}$