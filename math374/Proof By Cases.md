### $$(P_1\lor P_2)\rightarrow Q \Leftrightarrow (P_1\rightarrow Q)\land (P_2\rightarrow Q)$$ This can be expanded for any finite amount of P $$(P_1\lor P_2 \lor ...\lor P_n)\rightarrow Q \Leftrightarrow (P_1\rightarrow Q)\land (P_2\rightarrow Q)\land ...\land(P_n\rightarrow Q)$$
### Theorem:
#### $\forall x, y$  $|x*y| = |x|*|y|$

Proof by cases:
1. $x\ge 0, y\ge 0$  $P_1$
2. $x\ge 0, y\lt 0$  $P_2$
3. $x\lt 0, y\ge 0$  $P_3$
4. $x\lt 0, y\lt 0$  $P_4$

We prove each statement because these are all the possible cases for the theorem.

### Theorem:
#### $\forall n$ natural numbers, $n^2$ ends in 0, 1, 4, 5, 6, or 9 in decimal.

Proof by cases:
1. $n = 10k$
2. $n=10k +1$
3. $n=10k +2$
4. $n=10k +3$
5. $n=10k +4$
6. $n=10k +5$
7. $n=10k +6$
8. $n=10k +7$
9. $n=10k +8$
10. $n=10k +9$
$$(P_1)\lor(P_2)\lor ...\lor(P_{10})\Leftrightarrow T$$
If we want to show $P_9 \rightarrow$ 
$$n^2=(10k)^2 + 2(10k)*8 + 8^2 = 10(10k^2+16k+6) +4$$The answer ends in 4 which matches our theorem. This works for every other case as well.

