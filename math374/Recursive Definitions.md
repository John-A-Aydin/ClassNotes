We define something in the first step that is similar to the base case and make a recursive step.
Uses the same principles used when [[Correctness of Loops|proving a loop]].

### Sequences

$a_0 = 1$,    for $n \ge 0$  $a_{n+1} = 2a_n$ 
1. $a_1 = 2a_0 = 2$
2. $a_2 = 2a_1 = 4$
3. $a_3 = 2a_2 = 8$
Conjecture ($P(n)$):
	$a_n = 2^n$

Claim $\forall n\ge 0$, $P(n)$
	Base Case: $a_0 = 1$

Inductive step:
	$\forall n\ge 0$,   $P(n)\rightarrow P(n+1)$
$a_{n+1}$= $2a_n$ = $2*2^n$ = $2^{n+1}$


### String: 
- Elements of alphabet where order matters (word)

##### Empty String $\lambda$ or $\frac{\text{ }}{}$  

##### String Operations:
- Concatenation
	- $xy$ is the concatenation of x and y
	- $xy \ne yx$
	- $\lambda x = x \Leftrightarrow x\lambda = x$


### Palindromic Strings

Def. read the same from left to right as right to left

**Base Case:** 
$\lambda$
	or
any 1 letter word

**Recursive Step:**

$P(n+1)$ =  concat on the front and back of string $P(n)$

## Backus-Naur Form
#### Ex. 1 (BNF)

\<identifier> = \<letter> | \<identifier>\<letter> | \<identifier>\<digit>
	We need a base case (\<letter>)

Informal description:
	Can contain lowercase letter and digits of any length, but cannot start with a digit.

\<letter> = a | b | c | d | ... | z
\<digit> = 0 | 1 | 2 | 3 | ... | 9

#### Ex. 2 (BNF)

Words using only letters no consonant ever before a vowel

\<identifier> = \<vowel> | \<vowel>\<identifier> | \<identifier>\<consonant>
or
\<identifier> = $\lambda$ | \<vowel>\<identifier> | \<identifier>\<consonant>

#### Ex. 3 (BNF)

Words with no two consecutive vowels and no two consecutive consonants

\<identifier> = \<c-ending> | \<v-ending>

\<c-ending> = \<consonant> | \<v-ending>\<consonant>
\<v-ending> = \<vowel> | \<c-ending>\<consonant>

