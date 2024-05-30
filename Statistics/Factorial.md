$$\Large n! = n(n-1)(n-2)...(2)(1)$$
Factorials are useful when one outcome obstructs another outcome from happening for the next event
- Number of combinations of seating
- Probability of things sharing a quality
- 
##### Ex.
Finding the probability that a group of 10 people have at least 2 people who share a birthday ($P_S$).

$$P_S = 1-P_{!S}$$

We can reverse the question be checking the probability that no one shares a birthday.

$$P_S= 1-\frac{(365)(364)(363)...(365-10+1)}{(365)(365)(365)...(365)}$$

##### Number of ways you can pick n distinct objects k times without replacement
When the order matters:

$$\large nP_k= \frac{n!}{(n-k)!}$$

When order doesn't matter:

$$\large nP_k = \frac{n!}{k!(n-k)!}= (_{k}^{n})$$
