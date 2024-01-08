## LTI

#### Linear
- Scaling
	- $Cx(t)\rightarrow Cy(t)$
	- Any system with a term that does not include $x(t)$ is Non-Linear
- Additive

#### Time-Invariant
Given:
	$x(t) \rightarrow y(t)$
then:
	$x(t-T)\rightarrow y(t-T)$ 
- Look for floating t's that aren't in x(t)

### Examples

$\large y(t) = 3x(t)+1$
- Non-Linear
- Time-Invariant

$\large y(t) = 3sin(t)x(t)$
- Linear
- Not Time-Invariant

$\large \frac{dy}{dt} + ty(t) = x(t)$
- Linear
- Not Time-Invariant

$\large \frac{dy}{dt} + 2y(t) = 3\frac{dx}{dt}$
- Linear
- Time-Invariant

$\large y(t) = \int_{-\infty}^tx(\tau)d\tau$ 
- Linear
- Time-Invariant

$\large y(t) = \int_{0}^tx(\tau)d\tau$ 
- Linear
- Not Time-Invariant

$\large y(t) = \int_{t-1}^{t+1}x(\tau)d\tau$
- Linear
- Time-Invariant

### Examples from Review

$\large y(t) = 3x(t-1)$
- Linear
- Time-Invariant

$\large y(t) = tx(t)$
- Linear
- Not Time-Invariant

$\large\frac{dy}{dt} + y(t-1) = x(t)$
- Linear
- Time-Invariant

$\large\frac{dy}{dt} + 2y(t) = \int_{-\infty}^tx(\tau)d\tau$    ?
- Linear
- Time-Invariant

$\large y(t) = x(t)u(t)$     ?
- Linear
- Non Time-Invariant

$\large y(t) = \int_t^\infty x(\tau)d\tau$            ? 
- Linear
- No idea

$\large y(t) = \int^{2t}_t x(\tau)d\tau$              ?
- Linear ???
- Not Time-Invariant?????

## LTI Sinusoidal Response

$\large x(t) = 1+2cos(t)+3cos(2t)$
$\large y(t) = 6cos(t) + 6cos(2t)$

$A = \frac{0}1$,     $B = \frac{6}2$,     $C = \frac{6}3$

If 
$x(t) = X + Ycos(t) + Zcos(2t)$
Then
$y(t) = AX + BYcos(t) + CZcos(2t)$


## Impulse Response of RC 

$\Large h(t) = \frac{1}\tau e^{-t/\tau}u(t)$ 

$\Large V_{out}(t)  = V_{in}(t)*h(t) = \int_0^t V_{in}(\tau)h(t-\tau)d\tau$ 
 