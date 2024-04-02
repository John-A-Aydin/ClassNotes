Hash table that only allows one element per bucket

# Operations

### Deletions
When deleting elements we need to use grave markers to indicate that the slot was previously filled.
This indicates that the element we are looking for could be in a higher indexed bucket.

# Strategies
### Linear Probing
$\large h(k)\text{ , } h(k) +1\text{ , } h(k)+2 \text{ ...}$

When a collision occurs, place element in the next available bucket.

As the hash table starts to fill, clusters form.

### Double Hashing
$\large h(k)\text{ , } h(k) + s(k)\text{ , } h(k) + 2s(k) \text{ ...}$

The first hash function gives you an initial position and the second hash function gives a "stride". Instead of shifting the item 1 bucket over when a collision is detected, we will shift it by the stride

The main goal with this is to spread out the information.

### Quadratic Probing 
$\large h(k) \text{ , } h(k) + 1^{2} \text{ , } h(k) + 2^{2} \text{ ...}$


