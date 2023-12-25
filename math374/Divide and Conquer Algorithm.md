#2-5

### Ex. 1
#### MergeSort(L)

$\large L = L_1 \text{ and } L_2$
- Split L at the middle

MergeSort($L_1$)
MergeSort($L_2$)

##### Consider L = \{1, 8, 6, 5, 2, 4, 3, 7}

$L_1$ = \{1, 8, 6, 5}    $L_1^*$ = \{1, 5, 6, 8}
$L_2$ = {2, 3, 4, 7}   $L_2^*$ = \{12, 3, 4, 7}

Merge $L_1^* \text{ and } L_2^*$


### Ex. 2

#### Binary Search

$\large C(1) = 1$
$\large C(n) = C(\frac{n}2)+1$,      $\large n= 2^m \ge 2$

Solving this using [[Backtracking]]:

$C(\frac{n}2) = C(\frac{n}4) +1$ 
$C(\frac{n}4) = C(\frac{n}8) +1$
$C(\frac{n}2) = C(\frac{n}8) +1 + 1 + 1$

$\large C(n) = C(\frac{n}{2^k}) + k$

$\large C(\frac{n}{2^k}) = 1$  if  $\large k = log_2(n)$


### Ex. 3

$\large S(n) = CS(n/2)+ g(n)$
￼￼




