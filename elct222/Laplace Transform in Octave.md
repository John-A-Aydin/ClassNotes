```MatLab
pkg load symbolic
syms s t

f1t = some function of t

F1s(s) = laplace(f1t, t)
```

### Inverse Laplace

```Matlab
pkg load symbolic
syms s t

F1s = some function of s

f1t = ilaplace(F1s)
```