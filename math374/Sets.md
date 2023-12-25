#3-1 

Sets are unordered groups of things
- Think of it as a burlap sack containing elements

$\large a \in B$ 
- a is an element of B

$\large a \notin B$
- a is not an element of B

# Definitions
#### Equality of Sets

$\Large A = B$   $\Large\text{ if }$  $\Large \forall x(x\in A \leftrightarrow x\in B)$ 
$\Large A = B$   $\Large\text{ if and only if }$  $\Large (A\subset B)\land(B\subset A)$

#### Def. of Subset

$\Large C\subset B$  $\Large \text{ if }$  $\Large \forall x(x\in C \rightarrow x\in B)$

#### Def. of Proper Subset

$\Large \text{if }$$\Large (C\subset D)\land(C\ne D)$

# Important Sets

$\Large \mathbb{N}$
- Natural numbers
$\Large \mathbb{Z}$
- Integers
$\Large \mathbb{Q}$
- Rational numbers
$\Large \mathbb{R}$
- Real numbers
$\Large \mathbb{C}$
- Complex numbers
$\Large \emptyset$
- Empty set

# Example

1. 
	We have Universe $u$ 
	and a predicate $P(x)$

	$A = \{x | P(x)\}$ 

2. 
	universe $= \mathbb{R}$ 
	$P(x) = \{x^2-3x+2 = 0\}$

	$A = \{x|x^2-3x+2=0\} = \{1,2\}$

# Set Operations

[[Equivalence and Inference Rules]] often apply to set operations

Universe $\large u$
	$\large A, B \subset u$
	$\large A = \{ x|p(x)\}$
	$\large B = \{ x|q(x)\}$

#### Union $\large \cup$
	$\large A\cup B = \{x|p(x)\lor q(x)\}$

#### Intersection $\large \cap$
	$\large A\cap B = \{x|p(x)\land q(x)\}$

#### Complement $A'$
	$\large A' = \{x|p(x)'\}$ 

#### Difference $\large -$
	$\large A-B = \{x|\in A\text{, but } x\notin B\}$

#### Symmetric Difference (XOR) $\oplus$  
	$\large A\oplus B = \{(A-B)\cup(B-A)\} = \{x | p(x) \oplus q(x)\}$

#### Cartesian Product $\large \times$
	$\large A\times B = \{(u,v)|u\in A, v\in B\}$
	
	$\large \{1,2,3\}\times\{3,4\} = \{(1,3), (1,4), (2,3),(2,4),(3,3),(3,4)\}$ 

#### Binary Operation $\large \circ$ 
- it assigns to every $a\in A$, $b\in A$  or  $a\circ b$
- $a\circ b\in A$ 
- TLDR
	- $\forall a\in A$, $\forall b\in A$,  $\{a\circ b\in A\}$ 
	- The output must be in the same set as the inputs 
	**Examples:**
	 $A=\mathbb{N}$ 
	 - $\circ$ is subtraction
	 - $a\circ b$  means  $a-b$   
	 - $a-b$  could result in a negative number so this doesn't work

#### Unary Operation $\#$ 
- $\forall a\in A$    $\exists 'a^{\#}$
- $\forall a$  $a^{\#}\in A$
	**Examples:**
	$A = \mathbb{Z}$
	- $a^{\#} = -a$
	- This works as a unary operator
	$A=\mathbb{R}$
	- $a^{\#} = \frac{1}a$ 
	- This does not work because 1/0 does not exist
	$A=\mathbb{N}$
	- $a^{\#} = -a$
	- negative numbers do not belong in $\mathbb{N}$ 

### Cardinality

Two sets are cardinal if every item in set A can be associated with an item in set B