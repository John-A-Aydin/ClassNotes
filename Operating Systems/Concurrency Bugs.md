### Non Deadlock Bugs

#### Atomic Violation

The desired serializability among multiple memory accesses is violated. 
- We need to [[Locks|lock]] when writing
#### Order Violation

The desired order between two memory accesses is flipped.
- i.e. A should always be executed before B but the order is not enforced during execution
- Enforce ordering using condition variables


### Deadlock Bugs

- The presence of a cycle
	- Thread1 is holding a lock L1 and waiting for another one, L2
	- Thread2 holds lock L2 is waiting for L1 to be released
	- Occurs when threads need multiple locks

##### Why do deadlocks occur?
1. In large code bases, complex dependencies arise between components
2. Due to the nature of encapsulation
	-  Hide details of implementations and make software easier to build in a modular way
	-  Modularity does not mesh well with [[Locks|locking]]

##### Conditions for Deadlock

1. Mutual Exclusion
	- Threads claim exclusive control of resources that they require.
2. Hold-and-wait
	- Threads hold resources allocated to them while waiting for additional resources
3. No preemption
	- Resources cannot be forcibly removed from threads that are holding them.
4. Circular wait
	- There exists a circular chain of threads such that each thread holds one more resources that are being requested by the next thread in the chain

Breaking any one of these conditions stops deadlock

#### Prevention

- Provide a total ordering on lock acquisition
	- This approach requires careful design of global locking strategies
	- Ex. We can prevent deadlock by always acquiring L1 before L2

###### Hold and Wait
- Acquire all locks at once, atomically
	- Problem
		- Require us to know when calling a routine exactly which looks must be held and to acquire them ahead of time
		- Decreases concurrency

###### No Preemption
- When trying to get multiple locks we might hold on to one while waiting for another
- We can implement a trylock() function
- 