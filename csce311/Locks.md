
### The Basic Idea

##### Ensure that any critical section executes as if it were a single atomic instruction

##### Lock variable holds the state of the lock
- Available
	- No [[Threads|thread]] holds the lock
- Acquired
	- A [[Threads|thread]] holds the lock

### The Semantics of the lock()

##### lock()
- Try to acquire the lock
- If no other thread holds the lock, the thread will acquire the lock
- Enter the critical section
	- This thread is said to be the owner of the lock.
- Other threads are prevented from entering the critical section while the first thread that holds the lock is in there.
- use pthread_mutex_ t lock = PTHREAD_MUTEX_INITIALIZER;

### Building A Lock

- Efficient locks provided mutual exclusion at low cost
- Building a lock needs some help from the hardware and the OS

#### Basic Criteria
 1. **Mutual Exclusion**


### Ticket lock
(Slide 35)
- Built with fetch-and-add
- Fair
	- ensures every [[Threads|thread]] progresses 
- FIFO
- [[Context Switch|Context Switching]] still costs resources

### Avoiding Spinning
- Just give up the CPU to another thread

**Queue**
- park()
	- Put a calling thread to sleep
- unpark()
	- Let the calling thread run
- We spin when the thread has the guard
	- threads don't hold the guard for very long

##### Futex
(Slide 43)
- futex_wait(\<address>, \<expected>)
- futex_wake(\<)

##### Two-Phase Locks
- First phase
	- spins for a short time
	- second phase is entered
- Second phase
	- wait

