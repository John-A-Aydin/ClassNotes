Occurs when a [[System Call]] is made.
- Raises the privilege level to kernel mode
- Saves registers at the kernel stack
- Locates the destination in the kernel
- Jumps to the destination 
- Interrupts number for system call

#### Return-from-trap Instruction
- Return into the calling user program
- Reduce the privilege level back to user mode

#### Sources of traps
- Completion of disk I/O
- Keyboard interrupt
- System Call

#### Trap Handler
- The code to run for each interrupt number (trap number)

#### Trap Table
- Contains all the events the system looks out for eg. Division by 0, Illegaly accessing memory
- The address of the trap handlers
- Hardware informs the location of the trap table to OS when booting
- The instruction to inform the location of the trap table is also privileged instruction.
- You cannot execute this instruction in user mode.