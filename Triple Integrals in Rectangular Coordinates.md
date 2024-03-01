==**15.5**==

$$\large \int \int \int_{R} f(x,y,z) \text{ }dV$$
### Definition

First we assume that $\large R$ is a rectangular prism.

![[rectangular-prism.png]]

We divide the box shaped region into smaller boxes with volumes of

$\large \Delta V_{k} = \Delta x_{k} \Delta y_{k}\Delta z_{k}$

The hyper volume of a four dimensional box is:

$$\large f(x_{k}^{*}, y_{k}^{*},z_{k}^{*})\Delta V_{k}$$

Letting the number of boxes go to infinity and adding them up, we get:

$$\large \large \int \int \int_{R} f(x,y,z) \text{ }dV = \lim_{n\to \infty} \sum\limits_{k=1}^{n}\large f(x_{k}^{*}, y_{k}^{*},z_{k}^{*})\Delta x_{k} \Delta y_{k}\Delta z_{k}$$

### Differences Between Doubles and Triples

#### 1. Fubini's Theorem Still Applies

The order of integration does <u>not</u> change the result.

This means we now have 6 possible orders of integration which makes it harder to find the easiest order of integration.

##### Example

$\large \int \int \int_{B} x^{2}yz \text{ }dV$

where:

$\large B = \{(x,y,z) : 1\le x\le 2, 0\le y\le 1, 0\le z \le2\}$

All we have to do is pick and order. (it doesn't matter here)

$\large \int_{0}^{2}\int_{0}^{1}\int_{0}^{2} x^{2}yz \text{ }dx \text{ }dy \text{ }dz$

This integral is just a more tedious version of a normal integral
