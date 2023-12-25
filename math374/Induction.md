Proving infinitely many statements in finite time

$P(n)$ n is any natural number 

If we can show that P(1) implies P(2) and P(2) implies P(3) .... we can prove P(n)


### First Principle of Induction$$P(c)\land \forall k \ge c$$$$P(k)\rightarrow P(k+1)$$$$(\forall n\ge c) P(n)$$
##### Things to consider when looking for a solution
- We have to connect $P(n)$ and $P(n+1)$
- We need to establish a base case $P(c)$


#### Ex.

Theorem: $\forall n \ge 0 \text{, } 2|n^2=n$

Base case $P(0)$ $2|0$  True

Inductive step
$P(k+1) = 2|(k+1)^2-(k+1) = k^2 + k$ 

$(k+1)^2-(k+1)$ is even by def of even numbers


#### Ex.

There are \$3 and \$4 coins

Theorem: $\forall n \ge 6$ n can be paid in exact change

Base case: $P(6) : 6 = 3+3$

Inductive step:
$\forall k \ge 6 \text{, } P(k)\rightarrow P(k+1)$
$c=6$

we consider a fixed payment of k

We have two cases
	pile has a 3 -> we change a 3 to a 4
	pile has no 3 and at least two 4's -> we change two 4's for three 3's
	pile has no 3 and at most one 4 -> Nothing to do bc this cant happen

### Second Principle of Induction$$P(c)\land \forall k \ge c$$$$\Big[P(c)\land P(c+1) \land \text{ ... }\land P(k) \rightarrow P(k+1)\Big] \rightarrow \forall n \ge c$$