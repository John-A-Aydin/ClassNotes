$\Large A_1$
$\Large A_1 \lor A_2$

$\Large n\ge2$

$\large A_1\lor A_2\lor ...\lor A_{n+1}$
can be written as
$\large (A_1\lor A_2\lor...\lor A_n)\lor A_{n+1}$

## Inductive Proof

#### Base Cases:
$\large n=2$    $\large A_1\lor A_2$
$\large n=3$    $\large (A_1\lor A_2)\lor A_3 \Leftrightarrow A_1\lor(A_2\lor A_3)$ 

#### Inductive Step

We consider an arbitrary parenthesization of:
$A_1, A_2, ... A_{k+1}$ 

##### Cases:

$\large (\text{...})\lor(A_{k+1})$
	Follows the definition

$\large (A_{1})\lor (...)$
	We can switch the sides with comm law

$\large (...) \lor (...)$
	We can conclude that this is logically equivalent to
	$(A_1\lor ...\lor A_{p})\lor(A_{p+1}\lor ...\lor A_{k+1})$
	$\Updownarrow$
	$[(A_1\lor ...\lor A_{p})\lor(A_{p+1}\lor ...\lor A_{k})]\lor A_{k+1}$
	