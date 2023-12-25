(Running program)

- A process is loaded into memory and running while a program is just a file on a computer
- Interact with the [[Process API]]

### Composition
- Memory
	- Instructions
	- Data
- Registers
	- Program counter
	- Stack pointer
### Process Creation 
1. Load a program code into memory, into the address space of the process
	- Programs initially reside on disk in executable format
	- OS performs the [[Lazy Loading]] on process
2. The program's runtime [[Stack]] is allocated
	- A process' stack stores the local variables of the program 
	- Initialize the stack with arguments argc and the argv array of main() function
3. The program's [[Heap]] is created
	 - Used for explicitly requested dynamically allocated data
	 - Program request such space by calling malloc() and free it by calling free()
4. The OS does some other initialization tasks.
	- input/output ([[I/O]]) setup
		- Each process by default has three open file descriptors.
		- Standard input, output and error
5. Start the program running at the entry point, namely main().
	- The OS transfers control of the CPU to the newly-created process.
### Process States
1. Running
	-  A process is running on a processor
2. Ready
	- A process is ready to be run but for some reason the OS has chosen not to run it at this given moment
3. Blocked
	- A process has performed some kind of operation
	- When a process initiates an [[I/O Request]] to a disk, it becomes blocked and thus some other process can use the processor.
	
	![[process_state_transition.png]]

### [[Data Structures]]
- PCB ([[Process Control Block]])
	- A C-structure that contains information about each process
	- [[Register Context]]: a set of registers that define the state of a process
		- "Pausing" a program to run another in a [[Context Switch]] means saving the state of the registers (and leaving the memory alone)
- Process List
	- Ready processes
	- Blocked processes
	- Running processes
