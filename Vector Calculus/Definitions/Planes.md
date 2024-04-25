
There are two ways to find the eqn of a plane

1. A point on the plane and the normal vector
2. Three points that lie on the plane


# Finding the equation with a point and normal vector

The equation of the plane with normal vector $\large \vec{N} = \langle1,-1,1\rangle$ containing $\large P = (0,0,0)$ is found by connecting any arbitrary point on the plane $\large (x,y,z)$ to $\large P$
$$\large \langle x,y,z \rangle$$
The normal vector $\large \vec{N}$ is orthogonal to this vector
$$\large \vec{N} * \langle x,y,x \rangle = 0$$
$$\large \langle 1,-1,1 \rangle * \langle x,y,z \rangle = 0$$
$$\large x-y+z=0$$

# Finding the equation of a plane with three points

The three points can be used to create 2 vectors.

### Example

$\large P = (0,0,0)$
$\large Q = (1,1,0)$
$\large R=  (0,1,1)$

Using $\large P$, $\large Q$, and $\large R$, we can construct the following vectors

$\large \vec{PQ} = \langle 1-0, 1-0, 0-0\rangle = \langle1,1,0\rangle$
$\large \vec{PR} = \langle0-0, 1-0, 1-0 \rangle=\langle 0,1,1 \rangle$

The [[Vectors#Cross Product|cross product]] of these vectors yields a new vector $\large \vec{N}$, that is normal to the plane
$\large \vec{N} = \vec{PQ} \times \vec{PR}$
This can be found with the [[Determinant|determinant]]

$\large \vec{N} = \langle1,-1,1\rangle$

If 
$$$$

