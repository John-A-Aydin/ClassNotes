##### Workload Assumptions
- Each [[Job]] runs for the same amount of time 
- All jobs arrive at the same time
- All jobs only use the CPU (no I/O)
- The run-time of each job is known

##### Scheduling Metrics
1. Performance metric: Turnaround Time
	- The time 
2. f
3. Response Time
	- The time from when the job arrives to the first time it is scheduled

### First In, First Out (FIFO)
- Very easy to implement

	Example: 
	- A arrived just before B which arrived just before C
	- Each job runs for 10 seconds
	![[FIFO_scheduling.png]]

### Shortest Job First (SJF)
- Non-preemptive scheduler

	Example: 
	- All arrive at the same time. If they don't arrive at the same time, they are just done in the order they arrived.
	- A runs for 100 seconds, B and C run for 10 each
	![[SJF_scheduling.png]]
### Shortest Time-to-Completion First (STCF)
- Adds preemption to SJF

	Example:
	- A arrives at t=0 and needs to run for 100 seconds.
	- B and C arrive at t=10 and each need to run for 10 seconds
	![[STCF_scheduling.png]]

### Round Robin (RR)
- Time slicing [[Scheduling|scheduling]]
	- Run a job for a time slice and then switch to the next job in the run queue until the jobs are finished.
		- Time slice is sometimes called a scheduling quantum.
	- It repeatedly does so until the jobs are finished.
	- The length of a time slice must be a multiple of the timer-interrupt period

	Example:
	- A, B and C arrive at the same time.
	- They each wish to run for 5 seconds
	![[RR_scheduling.png]]
# Incorporating I/O
1. When a job initiates an I/O request.
	- The job is blocked waiting for I/O  completion.
	- The scheduler should schedule another job on the CPU.

2. When the I/O completes
	- An interrupt is raised.
	- The OS moves the process from blocked back to the ready state

![[IO_scheduling.png]]