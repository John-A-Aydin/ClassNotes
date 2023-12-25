#2-5 
Look at $\large a(n)$ and start looking back in the sequence

$\Large S(n) = C*S(n-1) + g(n)$

$\Large S(1)\text{, }C\text{, and the function {g} are given}$ 

Start Backtracking
- $S(n-1) = C*S(n-2)+g(n-1)$
Plug back in to $S(n)$
- $S(n) = C(C*S(n-2)+g(n-1)) + g(n)$
- $S(n) = C^2S(n-2) + C*g(n-1) + g(n)$

Continue Backtracking
1. $S(n) = C*S(n-1) + g(n)$
2. $S(n) = C^2S(n-2) + C*g(n-1) + g(n)$
3. $S(n) = C^3S(n-3) C^2g(n-2) + Cg(n-1) + g(n)$
...
$C^kS(n-k) +C^{k-1}g(n-k+1) ...$ 

$\large S(n) = C^{n-1}S(1) + C^{n-2}g(2) + C^{n-3}g(3) + \text{ ... }+ C^1g(n-1) + C^0g(n)$ 
or
$\large S(n)=  C^{n-1}S(1) + \sum_{i=2}^nC^{n-i}g(i)$



