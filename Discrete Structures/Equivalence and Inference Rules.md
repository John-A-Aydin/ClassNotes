#1-1 
### Equivalences (Both ways)
1. Commutative (comm) $$ P \lor Q \Leftrightarrow Q \lor P $$
2. Associative (ass)$$ (P\lor Q)\lor R \Leftrightarrow P \lor (Q\lor R) $$
	- Only applies when operators are the same
3. Distributive (dis)$$ P\lor (Q \land R) \Leftrightarrow (P\lor Q)\land(P\lor R)$$
	- Works with most combinations of operators
4. De Morgan $$ (A\land B)' \Leftrightarrow A' \lor B' $$ $$  (A\lor B)' \Leftrightarrow A' \land B' $$
5. Implication (imp)$$ P\rightarrow Q \Leftrightarrow P' \lor Q $$
6. Double Negation (dn) $$ (P')' \Leftrightarrow P$$
7. Definition of Equivalence (equ)$$ P\leftrightarrow Q \Leftrightarrow (P \rightarrow Q) \land (Q\rightarrow P)$$
8. Contraposition (cont) $$ P\rightarrow Q \Leftrightarrow Q' \rightarrow P'$$

9. Self Reference (self)$$ P \Leftrightarrow P \land P$$$$ P \Leftrightarrow P \lor P$$
10. Exportation (exp)$$ (P \land Q) \rightarrow R \Leftrightarrow P\rightarrow (Q\rightarrow R)$$
### Inferences (One way)
1. Modus Ponens (mp) $$ P, P\rightarrow Q \Rightarrow Q $$
2. Modus Tollens (mt)  $$ P\rightarrow Q, Q' \Rightarrow P' $$
3. Conjunction (con) $$ P,Q \Rightarrow P\land Q $$
4. Simplification (sim) $$ P\land Q \Rightarrow P, Q $$
5. Addition (add) $$ P \Rightarrow P\lor Q $$
6. Disjunctive Syllogism (ds)$$P\lor Q, P'\Rightarrow Q$$
7. Hypothetical Syllogism (hs)$$P\rightarrow Q, Q\rightarrow R \Rightarrow P\rightarrow R$$
8. Resolution 
	(a)$$ (P \lor C) \land (Q\lor C') \Rightarrow P \lor Q$$
	(b)$$ (P \lor C') \land (Q\lor C) \Rightarrow P \lor Q$$
	(c)$$ (P' \lor C) \land (Q\lor C') \Rightarrow P' \lor Q$$
	-  If P is false then (a) simplifies to
			$C \land (Q\lor C')\rightarrow Q$ 
	- If Q is false then (a) simplifies to
			$(P\lor C)\land C' \rightarrow P$

### Predicate Logic

The predicate logic rules implement the [[Existential Quantifier]] and [[Universal Quantifier]].

1. Universal Instantiation (ui)
	$$\forall xP(x)\Rightarrow P(x)$$
	$$\forall xP(x)\Rightarrow P(t)$$
	- Where t is a new variable
	$$\forall xP(x)\Rightarrow P(c)$$
	- Where c is a constant

2. Existential Instantiation (ei)$$\exists xP(x) \Rightarrow P(a)$$
	- Where a is is a single constant 
	- A should be a new constant name

3. Universal Generalization (ug)$$P(x)\Rightarrow \forall xP(x)$$
	- $P(x)$ has not been (see textbook / lookup)

4. Existential Generalization (eg)$$(P(x)\lor P(a))\Rightarrow \exists xP(x)$$
	- If we start with $P(a)$, $x$ should not be present in $P(a)$ (applies when there are two variables)