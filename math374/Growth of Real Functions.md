#4-4 

### $\large \Theta$ def.
$\large f(n) = \Theta(g(n))$
if
$\large \exists (n_{0}\text{, }c_{1}\gt0\text{, }c_{2}\gt 0) \text{ such that }\forall (n\ge n_{0})\text{, }\text{ } c_{1}f(n)\ge g(n)\ge c_{2}f(n)$ 

#### Example

$\large n^{2}= \Theta(\frac{1}{2}n^{2}+5n)$

$\large c_{1}n^{2}\ge \frac{1}{2}n^{2}+5n\ge c_{2}n^{2}$

$\large c_{1} = \frac{1}{2}\text{, }n_{0} = 5\text{, }c_{2} = 5.5$


### $\large \Theta$ is an equivalence relation
$\large f(n) = \Theta(g(n)) \Rightarrow g(n)= \Theta(f(n))$

$\large \Theta$ is a symmetric and transitive relation


### $\large O$ def
$\large f(n) = O(g(n))$

$\large \text{if }\exists n_{0}\text{, }\exists c \gt 0$
$\large \forall n\gt n_{0}$
$\large f(n)\lt c*g(n)$

$\large \frac{f(n)}{g(n)}\lt c$

#### Claim:
$\large f(n) = \Theta(g(n)) \text{ if and only if } f(n) = O(g(n))\text{ and }g(n) = O(f(n))$

