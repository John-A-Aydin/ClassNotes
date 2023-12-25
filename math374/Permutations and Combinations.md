#3-4
## Permutation
### Notation:$$\large P(n,r) = \text{\# r-permutations of n elements}$$
### Some General Rules

$\Large P(n,n) = n!$

$\Large P(n, r) = n(n-1)(n-2)...(n-r+1) = \frac{n!}{(n-r)!}$ 

#### Ex. 1
n = 3 elements:  a, b, c

2-permutations: ab, ac, ba, bc. ca, cb

#### Ex. 2
How many anagrams of FISH
\= P(4,4) = 4!

####  Ex. 3
How many anagrams of MATTEL
$\ne P(6,6)$  because of the duplicate T's
$=6!/2! = 6!/2$ 

#### Ex. 4
How many anagrams of MISSISSIPPI

Look at the word like this $MI_1S_1S_2I_2S_3S_4I_3P_1P_2I_4$
We have 11 distinct letters now
\# of anagrams with subscripts = 11!

We think about grouping the subscripted anagrams into groups where the word are the same if the anagrams are removed. The number of groups will tell us the number of unsubscripted anagrams. How big are each of these groups?

We have 4 I's so how how many ways can we renumber the 4 I's? 4!
S's? 4!
P's? 2!

So the answer is 
\# of groups $\Large = \frac{11!}{4!4!2!}$ 


## Combination

### Notation: $$\large C(n,r) =^n_r =  \text{\# r-combinations of n elements}$$
### Some General Rules

$\large ^n_0 = 1$

$^n_n = 1$

#### Symmetry Rule

$\large ^n_k = ^n_{n-k}$ 

$\large ^n_k = \frac{n!}{k!(n-k)!}$ 


#### Ex. 1

n = 3,  {a, b, c}

2-combinations of 3 elements: {a,b}, {a, c}, {b, c}
