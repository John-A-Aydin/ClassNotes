$$\Large \delta (t-t) \text{   for  } t\ne T$$and$$\Large \int_{-\infty}^{\infty} \delta(t-T)dt= 1$$

### Sampling Property of $\delta(t)$
$$\Large \int_{-\infty}^{\infty} x(t)\delta(t-T)dt=x(T)$$


### In Matlab
##### Evaluate $\large \int_1^2 t^2$ 
```MatLab
clear all; clc;
pkg load symbolic;
syms t;

f = t^2*dirac(2*t-3);

G0 = int(f, t, 1, 2);
G0v = eval(G0);
```