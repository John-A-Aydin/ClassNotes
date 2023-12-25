#3-3 

N pigeons go into M pigeonholes
Then some hole has at least $[\frac{N}M]$pigeons

(if we have more pigeons than holes, there must be more than on pigeon in one of the holes)

#### Ex. 1

Given any 5 ints 
	Some 1 or more ints add up to a multiple of 5

Proof: 
$a_1$
$a_1+a_2$
$a_1+a_2+a_3$ 
...
...

If any of the 5 sums are a multiple of 5 we are done

If we take sum % 5 we get 1 | 2 | 3 | 4 

Pigeon Hole principle tells us that 2 sums will give the same remainder if divided by 5

3, 7, 18, 9, 2

$a_1+a_2+a_3+a_4 = 5l+r$
$a_1+a_2 = 5k + r$
$a_3+a_4= 5(l-k)$

This can be generalized to:
 Given any n ints
	 Some 1 or more ints add up to a multiple of n

#### Ex. 2 

**Theorem:**
Given 51 numbers from \[1,100]
	one of them divides another

**Proof:**

any $n\ge 1$,  can be written as $n = 2^m*b$ ,  where b is odd

Now we think of every possible value of b
	b can be any odd number between 1 and 99 (50 possibilities)

We have 51 numbers so two of them must have the same odd part

