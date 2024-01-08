
Adding [[Locks]] to a data structure makes the data structure thread safe
- Allows it to be used in multiple threads
- How locks are added determine both the correctness and performance of the data structure

The lock is acquired when calling a routine that manipulates the data structure


### Sloppy Counter
Tolerates error to prevent frequent access to the global counter

- Each [[Threads|thread]] keeps track of a list of how much has been done (logical counter)
- There is one global counter

When a thread wishes to increment the counter
- it updates the local counter
- Periodically transfers the local values to the global counter
- Less frequent updates of the global value can create more lag in the global value (sloppiness)
- More frequent updates make the counter act more like a single threaded thingy
