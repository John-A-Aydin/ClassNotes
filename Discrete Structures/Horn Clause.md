- Or of Predicates / Negated Predicates
- At most one predicate is not negated
- Used to simplify relations used in [[Programming Languages]]

### Ex. 
- $P(x)$ 
	- Horn
- $P(x)\lor Q(x)$
	- Not Horn
- $P(x)\lor (R(y))'$
	- Horn
- $A(x)\land (B(x))'$
	- Not Horn

##### Converting Statements to Horn Clauses

x is Prey if $E(x, y)\land A(x)$
1. $E(x, y)\land A(x)\rightarrow Prey(x)$
2. $(E(y, x)\land A(x))'\lor Prey(x)$
3. $E'(x, y)\lor A'(x)\lor Prey(x)$
	- This statement is now a horn clause
	- From the [[Equivalence and Inference Rules]] we can use Resolution
If we use this to check $E(b, f_i)$
1. $E(b, f_i)\land\ \left(E'(x, y)\lor A'(x)\lor Prey(x)\right)$
2. 
##### Resolution with Horn Clauses
##### $$(A\lor C')\land(B'\lor C)\rightarrow A\lor B'$$
The negation of *A* and *B* do not effect the usage of Resolution
