The goal here is to prove all of the variables as either true or false
We can use the [[Equivalence and Inference Rules]] to simplify and prove the statements
##### $$ A \land (B \rightarrow C) \land [(A\land B) \rightarrow(D \lor C)] \land B \rightarrow D $$
1. A hyp
	- Assuming A is true
2. $B\rightarrow C$ hyp
	- If B then C
3. $(A \land B) \rightarrow (D \lor C')$ hyp
	- If A and B then D or C'
4. B hyp
	- Assuming B is true
5. $A \land B$ 1,4 con
	- Using one and four we can say A and B are true
6. C
	- Using 2 and 4 we can say C is true (mp) 
	- If B is true then C is true
7. $D \lor C'$
	- Using 5 and 3 we can say that D or C' are true (mp)
8. D
	- Using 6 and 7 we can say that D is true (ds)


##### $$ [(A \lor B')\rightarrow C] \land (C\rightarrow D) \land A \rightarrow D$$
1. $(A \lor B') \rightarrow C$
	- Hypothesis
2. $C\rightarrow D$
	- Hypothesis
3. A
	- Hypothesis
4. $A\lor B'$
	- Using 3 (odd)
5. C
	- Using 4 and 1 we get C (mp)
6. D
	- Using 5 and 2 we get D (mp)

##### $$ (A' \lor B)\land (B\rightarrow C) \rightarrow (A \rightarrow C)$$
Using Deduction Method:
	$$ (A' \lor B)\land (B\rightarrow C) \rightarrow (A \rightarrow C) \Leftrightarrow (A'\lor B) \land (B\rightarrow C) \land A \rightarrow C$$
1. $A' \lor B$
	- Hypothesis
2. $B \rightarrow C$ 
	- Hypothesis
3. A
	- Hypothesis
4. B
	- Using 1 and 3 (ds)
5. C
	- Using 4 and 3 (mp)