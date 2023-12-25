
Transforming a signal into the summation of several sin and cos signals

**The Fourier theorem states that a periodic function f(t)
of period T can be cast in the form

$$\Large f(t)= a_{0}+\sum\limits^{\infty}_{n=1}a_{n}cos(n \omega_{0}t) + b_{n}sin(n \omega_{0}t)$$
$$\large\omega_{0}= \frac{2 \pi}{T}$$$$\large a_{0} = \frac{1}{T}\int_{0}^{T}f(t) dt$$
$$\large a_{n}=\frac{2}{T}\int_{0}^{T}f(t)cos(n \omega_{0}t)dt$$
$$\large b_{n}= \frac{2}{T} \int_{0}^{T}f(t) cos(n \omega_{0}t)dt$$
**Alternatively:**
$$\Large f(t)= a_{0}+\sum\limits^{\infty}_{n=1}A_{n}cos(n \omega_{0}t + \phi_{n})$$
$$\large A_{n}= \sqrt{a_{n}^{2}+b_{n}^{2}}$$
$$\large\phi_{n} = -tan^{-1}\left(\frac{b_{n}}{a_{n}}\right)$$

### Number of terms (n)

We can choose how many terms to use
more terms makes it more accurate