
Let $\large \vec{F}(x,y,z) = \langle M(x,y,z), N(x,y,z), P(x,y,z) \rangle$
Recall that $\large \nabla$ is
$$\large \nabla = \Big\langle \frac{\partial }{\partial x}, \frac{\partial }{\partial y}, \frac{\partial }{\partial z} \Big\rangle$$
Then the divergence of $\large \vec{F}$ denoted $\large \text{div}\vec{F}$ is
$$\large \text{div}\vec{F} = \nabla \cdot \vec{F} =  \frac{\partial M}{\partial x} +  \frac{\partial N}{\partial y} + \frac{\partial P}{\partial z} $$




Suppose that $\large \vec{F}$ is the velocity field of a fluid

Then $\large \text{div}\vec{F}(p)$ measures the tendency of the fluid to move away from $\large p$ if
$\large \text{div}\vec{F}(p) \gt 0$  ($\large p$ is a <u>source</u>)
and towards $\large p$ if
$\large \text{div}\vec{F}(p) \lt 0$  ($\large p$ is a <u>sink</u>)

If $\large \text{div}\vec{F}(p) = 0$, then the fluid is <u>incompressible</u> at $\large p$

# Examples

### Example 1
Find the divergence of $\large \vec{F}$ where:
$$\large \vec{F}(x,y,z) = \langle x^{2}yz, 3xyz^{3}, x^{2}-z^{2} \rangle$$
$$\large \text{div}\vec{F} = \frac{\partial }{\partial x}(x^{2}yz) + \frac{\partial }{\partial y}(3xy^{3}) + \frac{\partial }{\partial z}(x^{2}-z^{2})$$
$$\large \text{div}\vec{F} = 2xyz+ 3xz^{3}+ -2z$$

### Example 2

Find
$$\large \text{div}(\text{curl}(\vec{F}))$$
$$\large \text{curl}\vec{F} = \Big\langle P_{y} - N_{z}, M_{z} - P_{x}, N_{x} - M_{y} \Big\rangle $$
$$\large \nabla (\nabla \times \vec{F}) = P_{yx} - N_{zx} + M_{zy} - P_{xy} + N_{xz} - M_{yz} = 0$$

$\large $