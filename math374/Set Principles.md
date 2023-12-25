#3-2
[[Sets]]

## Sum/Addition Principle

If we can do something in
$n_1, n_2, n_3, ... n_k$ distinct ways
then the total number of ways is
$n_1 + n_2+n_3+...+n_k$

Number of sets $A_1, A_2, ... , A_k$
If
$\forall i<j$  $A_i\cap A_j = \emptyset$
Then
$|A_1\cup A_2\cup ... \cup A_k|$  =  $A_1 + A_2 + ... + A_k$

## Product/Multiplication Principle

Creating some objects is broken down into $k$ steps such that
- steps have $n_1, n_2, ...,n_k$ outcomes
- by this steps every object is created and is created only once
Then
\# of objects = $n_1 n_2 ... n_k$


$x\in A_1\times A_2\times A_3$
$x=(a_1 a_2 a_3)$
	$a_1 \in A_1$
	$a_2 \in A_2$
	$a_3 \in A_3$
$|A_1\times A_2 \times A_3| = |A_1||A_2||A_3|$


## Complement Principle$$\large |A| = |u|-|A'|$$
##### Ex.
We want to know how many combinations of 5 letter alphabetical strings can be created with some amount of repetition

$u=$ total number of 5 letter words $= 26^5$
$A' =$ number of 5 letter words with no repetition $= (26)(25)(24)(23)(22)$

So 
$A = 26^5 - (26)(25)(24)(23)(22)$

## [[Pigeon Hole Principle]]

## Example Problems

#### 1. 
How many 4 digit numbers start with 4 or 5?

The first digit of a four digit number can be filled out 2 different ways (4 or 5)
The next digits have 10 possibilities each

So
$(2)(10^3)$ 

#### 2. 
A card deck is really just ordered pairs so we can represent it as a [[Cartesian Product]]
Card deck $= \{A,2,3,,..,10,J,Q,K\}\times\{Hearts, Clubs, Diamonds, Spades\}$
