Predicate logic incorporates Quantifiers like the [[Existential Quantifier]], [[Universal Quantifier]], and ...

##### Ex. 1
	"Every  human is mortal."
	"Socrates is a human."
	"Therefore, Socrates is mortal."

- x is a breathing being (universe)
- x is human   $H(x)$
- x is mortal    $M(x)$
$$(\forall x(H(x)\rightarrow M(x)))\land H(s)\rightarrow M(s)$$
Using a combination of the [[Equivalence and Inference Rules]] and 
 1. $\forall x(H(x)\rightarrow M(x))$ (hyp)
 2. $H(s)$ (hyp)
 3. $H(s) \rightarrow M(s)$ (universal instantiation)
 4. $M(s)$ (mp)

##### Ex. 2
$$[\forall xP(x)\rightarrow Q(x)]\land (\forall xP(x))\rightarrow(\forall xQ(x))$$
Proof Sequence:
1. $\forall x P(x)\rightarrow Q(x)$ (hyp)
2. $\forall xP(x)$ (hyp)
3. $P(x)\rightarrow Q(x)$ (1, ui)
4. $P(x)$ (2, ui)
5. $Q(x)$ (3, 4, mp)
6. $\forall xQ(x)$ (5, ug)

##### Ex. 3
$$\forall x P(x)\rightarrow \exists xP(x)$$
Proof Sequence:
1. $\forall xP(x)$ (hyp)
2. $P(x)$ (1, ui)
3. $\exists xP(x)$ (2, eg)

##### Ex. 4
$(\exists xP(x))\lor (\exists xQ(x))$ (hyp)
$P(a)\lor Q(a)$ (Illegal)
