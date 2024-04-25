Let $\large \vec{F}(x,y,z) = \langle M(x,y,z), N(x,y,z), P(x,y,z) \rangle$
Recall that $\large \nabla$ is
$$\large \nabla = \Big\langle \frac{\partial }{\partial x}, \frac{\partial }{\partial y}, \frac{\partial }{\partial z} \Big\rangle$$
Then the curl of $\large \vec{F}$ denoted $\large \text{curl}(\vec{F})$ is
$$\large \text{curl}(\vec{F}) = \nabla \times \vec{F} = \text{det}\begin{bmatrix} \hat{i}  & \hat{j} & \hat{k}  \\ \frac{\partial}{\partial x} & \frac{\partial }{\partial y} & \frac{\partial }{\partial z}  \\ M & N & P & \end{bmatrix}$$
or
$$\large \text{curl}(\vec{F}) = \Big \langle \frac{\partial P}{\partial y} - \frac{\partial N}{\partial z}, \frac{\partial M}{\partial z} - \frac{\partial P}{\partial x}, \frac{\partial N}{\partial x} - \frac{\partial M}{\partial y} \Big\rangle$$
To solve this we have to write the [[Cross Product|cross product]] as a [[Determinant|determinant]].

Suppose that $\large \vec{F}$ is the velocity field of a fluid
Then $\large \text{curl}\vec{F}(p)$ tells us the direction of the axis about which the fluid rotates most rapidly.

# Examples 

### Example 1
Find the curl of $\large \vec{F}$ where:
$\large \vec{F}(x,y,z) = \langle x^{2}yz, 3xyz^{3}, x^{2}-z^{2} \rangle$
$$\large \text{curl}\vec{F}= \nabla \times \vec{F} = \text{det}\begin{bmatrix} \hat{i}  & \hat{j} & \hat{k}  \\ \frac{\partial}{\partial x} & \frac{\partial }{\partial y} & \frac{\partial }{\partial z}  \\ x^{2}yz & 3xyz^{3} & x^{2}-z^{2} & \end{bmatrix}$$
$$\large \text{curl}\vec{F} = \langle -9xyz^{2}, - (2x-x^{2}y), 3yz^{3}-x^{2}z \rangle$$
