

- Used when a [[Process]] would benefit from multiple CPU cores for performance reasons
- Require assurances that two threads don't try to access the same data at the same time
- Each thread has its own [[Stack]]

A new abstraction for a single running process

**Multi-threaded program**
- Has more than one point of execution
- Multiple Program Counters
- Share the same address space

### [[Context Switch]] between threads

**Each thread has its own program counter and set of registers**
- One or more Thread Control Block are needed to store the state of each thread

**When switching from running one (T1) to running the other (T2),**
- The register state of T1 be saved.
- The register state of T2 restored.
- The address space remains the same

### Why use Threads?

**Parallelism**
- Single-threaded program: the task is straightforward, but slow.
- Multi-threaded program: natural and typical way to make programs run faster on modern hardware.
- Parallelization: The task of transforming standard single-threaded program into a program that does this sort of work on multiple CPU's.

**Avoid blocking program progress due to slow I/O.**
- Threading enables overlap of I/O with other activities within a single program.
- It is much like multi programming did for processes across programs.

**Separate unrelated Logic into cohesive parts: Complicated programs are composed of separate logics that have little to do with one another. Consider a game:**
- Drawing has little to do with playing audio or handling keyboard input.
- BUT they are not entirely unrelated. It is likely that there is a central loop that is controlling/coordinating everything.
- The actual design is cleaner but logic interactions may be problematic.
- Parallelism for performance is often a single task/logic, so is different.

**When considering threads, you need to consider**
- What logic is separable from other logic.
- Where the separate logics interact with one another. ==Decoupling==

### Some C++ Code

##### Thread Creation

```C++
 #include <stdio.h>
 #include <assert.h>
 #include <pthread.h>
 #include “common.h”
 #include “common_threads.h”
 
 void *mythread (void *arg) {
     printf (“%s\n”, (char *) arg);
     return NULL;
 }
 
 int main (int argc, char *argv[]) {
     pthread_t p1, p2;
     int rc;
     printf(“main: begin\n”);
     Pthread_create(&p1, NULL, mythread, “A”);
     Pthread_create(&p2, NULL, mythread, “B”);
     // join waits for thre threads to finish
     Pthread_join(p1, NULL); // Join acts like an await statement in JS
     Pthread_join(p2, NULL);
     printf(“main: end\n”);
     return 0;
 }
```

##### Sharing Data

```C++
int max;
volatile int counter = 0; // shared global variable

void *mythread(void *arg) {
	char
}
```


### A Few Terms

##### Race Condition
- The results depend on the timing execution of the code
- Result is indeterminate

##### Critical Section
- A piece of code that accesses a shared variable and must not be concurrently executed by more than one thread
- Multiple threads executing critical sections can result in a ==Race Condition==
- Need to support atomicity for critical sections (mutual exclusion)