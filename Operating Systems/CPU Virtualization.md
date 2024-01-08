- The OS promotes the illusion that many different CPU's exist
- [[Time Sharing]] is used to achieve more virtual CPU's than cores

### Regaining control of the CPU

##### Cooperative Approach: Wait for [[System Call]]s
1. Processes periodically give up the CPU by making system calls such as yield
	- The OS decides to run some other task 
	- Application also transfer control to the O when they do something illegal
##### Non-Cooperative Approach: OS Takes Control
1. A timer interrupt
	- During the boot sequence, the OS starts a timer
	- The timer raises an interrupt every few milliseconds
	- When the interrupt is raised:
		- The currently running process is suspended
		- Save enough of the state of the process
		- A pre-configured interrupt handler in the OS runs


### Types of Execution

##### Limited Direct Execution
- The process runs on the CPU
- The process is limited on what it can do and doesn't have full control over the computer