### Main Idea
Solve smaller overlapping sub problems
Record solutions to sub problems so that each is only solved once (==memoization==)


### Example: Fibonacci

$\large f(0) = 0$
$\large f(1)= 1$
$\large f(n) = f(n)+f(n-1)$

Trying to compute a Fibonacci number using the definition, creates an unreasonable order of growth.

A straight forward approach would be to go bottom up

### Example: Coin-row Problem

There is a row of $\large n$ coins whose values are some positive integers $\large c_{1}\text{, }c_{2} \text{ ... }$ not necessarily distinct. The goal is to pick up the maximum amount of money subject to the constraint that no two coins adjacent in the initial row can be picked up.

e.g. : 5, 1, 2, 10, 6, 2

Let $\large F(n)$ 

### Example: Transitive Closure

Take an adjacency matrix and turn it to a transitive closure
$\large M_{ij}$ is 1 if there is a path between nodes and 0 if there is no path