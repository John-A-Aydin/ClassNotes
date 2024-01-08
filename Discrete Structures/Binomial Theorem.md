#3-6
$$\Large (a+b)^n = \sum^n_{i=0}(_i^n)a^ib^{n-i}$$
Trick for finding $\large (a+b)^n$

$\large (a+b)^2 = aa + ab + ba + bb$
$\large (a+b)^3 = aaa + aab + aba + baa + abb + bab + bba + bbb$

They are just all the n letter words you can make with a and b

How many have:
	i a's
	n-i b's


#### Coefficient extraction operation
$\large p(x) =2+x^4+3x^5-x^7$

we look at each coefficient for p(x)
$[x^5]p(x)=3$
$[x^1]p(x) = 0$
$[x^0]p(x) = 2$
...

**Ex 1. 
$[x^3](x^3+x)^{100} = ????$

We can use the binomial theorem

$\Large = \sum_{i=0}^{100} (_i^{100}) x^{3i} x^{100-i}$ 

**Ex. 2

$[x^4](3x-5)^6$

$\Large \sum^6_{i=0} (_i^6) 3^ix^i(-5)^{6-i}$


**Ex. 3

$\large [x^{40}](x+1/x)^{100}$

a = x,  b = x^-1

$\Large \sum_{i=0}^{100} (_i^{100})x^i(x^{-1})^{100-i}$

$\Large= \sum_{i=0}^{100} (_i^{100})x^i(x^{i-100}$ 

$\Large =  \sum_{i=0}^{100} (_i^{100})x^{2i-100}$ 

we figure out when the $2i -100 = 40$
this happens at 70 so

$\large [x^{40}](x+1/x)^{100} = (_{70}^{100})$ 


$$\Large n2^{n-1} = \sum^n_{i=1} i(_i^n)$$
