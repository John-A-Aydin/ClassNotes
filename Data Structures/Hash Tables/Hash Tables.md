Data structure that stores key-value pairs.
Hash tables always have way less buckets than the number of possible keys.

A good hash table will minimize the number of buckets and bucket size.

### Terminology

##### Bucket
- Similar to an element in an array
- Can contain multiple values depending on structure of hash table

##### Hash Function
- The function that processes the input data
	- Usually converts input data to some integer corresponding to a bucket

##### Collision
- When two pieces of input data are assigned to the same bucket
- When dealing with collisions we can either use [[Open Hashing]]  or  [[Closed Hashing]]  


