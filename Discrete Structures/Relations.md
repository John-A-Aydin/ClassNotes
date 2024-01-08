#4-1 

## Binary Relations
A relation that can be either true or false

We denote relations with $\varrho$ or $\sigma$ 

We can think of a relation as taking an ordered pair from one or two sets where we apply the relation to each pair. 

To check the relation on every element of two sets we just check each pair in the [[Cartesian Product]] of the two sets

#### Ex. 
$\varrho \subseteq S\times T$,    $s\varrho t\text{   } (s\in S, t\in T)$ 

### Different Types of Binary Relations

#### One to One
- For any element in S there is one or none in T that share the relation

#### One to Many
- An element in S can have relation with many  things in F

#### Many to One
- An element in S can have relation with one thing in F, but elements of F can have many S relations


## Union $\cup$ 



## Intersection $\cap$


#### Ex. 
$\large \mathbb{R}\times\mathbb{R_{1}}, \le$   
$\large x\le y$,    $\large\le \subset \mathbb{R}\times \mathbb{R}$

$\large\mathbb{Z}\times \mathbb{Z_{1}}$,     $|$
$\large n|m$

$X$ is a set
$P(X)\times P(X)$
$\subseteq$  

### Properties of Binary Relations
1. Reflexivity$$\Large\forall s\in S\text{, }s\sigma s$$$$\large\forall a \in S \text{,  } (a,a)\in \sigma$$
	- Reflexive:
		- $\le$
		- $|$
		- $\subseteq$
	- Not Reflexive
		- $\lt$
		- $\subset$
	
2. Symmetric$$\Large\forall a\in S\text{, }\forall b \in S (a\sigma b\rightarrow b\sigma a)$$$$\large\forall a\in S\text{, }\forall b \in S \text{, } ((a,b)\in \sigma \rightarrow (b,a)\in \sigma)$$
	- Symmetric:
		- $=$
	- Not Symmetric:
		- $|$
		- $\le$
		- $\subseteq$
3. Transitivity$$\Large \forall x\in S \text{, }\forall y\in S \text{, }\forall z \in S(x\sigma y \land y\sigma z\rightarrow x\sigma z)$$$$\large \forall x\in S \text{, }\forall y\in S \text{, }\forall z \in S \text{, } ((a,b)\in \sigma\land (b,c)\in \sigma \rightarrow (a,c)\in \sigma)$$
	**Ex
	$(a<b)\land (b<c) \rightarrow a<c$ 
	- Transitive:
		- $\le$
		- $|$
		- $\subseteq$
		- $=$
		- $S = \{a, b, c, d, e, f\}$
			$\sigma = \{(d,e), (a,b), (b,c), (a,c)\}$
			Notice (a,b) and (b,c), that means (a,c) needs to be in $\sigma$ for the relationship to be transitive
4. Anti-symmetry$$\Large\forall a\in S, \forall b\in S \text{, } (a \sigma b\land b \sigma a \rightarrow a = b)$$
	- A relation can be Anti-symmetric and not Anti-symmetric at the same time
	- Anti-symmetric
		- $\le$
		- $\ge$
		- $=$
		- $\subseteq$

idrk what this is
$$\forall x\in S \text{, }[x] = \text{ equivalence of x }= \{y\in S| x\sim y\}$$


### Closure of binary relations

For a property P, (reflexive, symmetric, transitive ...)

Assume:
$\large\varrho  \subseteq S \times S$


$\large \sigma \subseteq S \times S$
and
$\large\varrho \subseteq \sigma$
and
$\large\sigma \text{ has property } P$
and
$\large\forall \gamma \subseteq S \times S$   if   $\large\varrho \subseteq \gamma\text{ and } \gamma \text{ has property P} \rightarrow \sigma \subseteq \gamma$ 


#### P = asymmetric
There is no asymmetric closure

$\large \mathbb{Z}$, divisibility

Recall the def of anti-symmetry

since $-2 | 2$ holds, antisymmetry fails


#### P = reflexivity, symmetry, or transitivity

Closure for property P exists

**Proof**

$\varrho \subseteq S \times S$

Reflexive Closure: $\large\varrho \cup \{(a, a)|a\in S\}$
- 

Symmetric Closure = $\varrho \cup \{(b,a)|(a,b)\in \varrho\}$

Transitive Closure:
- We keep adding pairs
- (a,b), (b,c) then add (c,d), (d,e) and so on
- 