
##### Ex. 

We have a number x and we want to compute $\sqrt{x}$ with the code *P* so $y = P(x)$
- The expectation is that $y^2 = x$
- $\forall x R(x, P(x))$
- $\forall x (P(x)^2 = x)$
	- $\forall x$ is really $\forall x>0$ since we are sqrting
- Q is a requirement for x

##### Hoare Triple
$$\{Q\} P \{R\}$$
- Q and R are statements
	- Q is a statement about the variables before the program runs
	- R is a statement about the input and output of the program
- P is the program
- Traversal:$$\{Q\}, e_1, \{Q_1\}, e_2, \{Q_2\}, ..., e_{k-1}, \{Q_{k-1}\}, e_k, \{R\}$$
	- We are verifying every line of the program
##### $$l_i$$
- In each iteration we are saying $x\leftarrow e$ (write e into x)
- 