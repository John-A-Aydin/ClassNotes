==**13**==
### Unit Tangent Vector
If $\large \vec{r}(t) = \langle x(t), y(t), z(t) \rangle$ represents the psition of an object, then 
$\large \vec{r}'(t) = \langle x', y', z' \rangle$ represents the velocity

The unit tangent vector $\large \vec{T}(t)$ to a smooth curve C is:
$$\large \vec{T}(t) = \frac{\vec{r}'(t)}{||\vec{r}'(t)||}$$

$\large \vec{T}(t)$ is the direction of motion

### Principle Unit Normal Vector

The principle unit normal vector is calculated with the [[Tangent and Normal Vectors of VVF|unit tangent vector]]
$$\large \vec{N}(t) = \frac{\vec{T}'(t)}{||\vec{T}'(t)||}$$
$\large \vec{N}(t)$ points in the direction the object is turning

### Example 1

Find the unit tangent vector and principle unit normal vectors of the path
$\large \vec{r}(t)  \langle \cos(t), \sin(t), t \rangle$

$\large \vec{r}'(t) = \langle - \sin(t), \cos(t) , 1\rangle$
$\large ||\vec{r}'(t)|| = \sqrt{(-\sin(t))^{2} + \cos^{2}(t) + 1^{2})} = \sqrt{2}$

so

$\large \vec{T}(t) = \Big \langle \frac{-\sin(t)}{\sqrt{2}} ,\frac{\cos(t)}{\sqrt{2}}, \frac{1}{\sqrt{2}} \Big \rangle$
and

$\large \vec{T}'(t) = \Big \langle \frac{-\cos(t)}{\sqrt{2}}, \frac{-\sin(t)}{\sqrt{2}}, 0 \Big \rangle$

$\large ||\vec{T}'(t)|| = \frac{1}{\sqrt{2}}$
so
$\large \vec{N}(t) = \langle -\cos(t), -\sin(t), 0 \rangle$
