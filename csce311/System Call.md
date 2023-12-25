Allow the [[Kernel]] to expose key pieces of functionality to user programs
- Accessing the file system
- Creating and destroying [[Process]]es
- Communicating with other [[Process]]es
- Allocating more memory

When a system call occurs a [[Trap Instruction]] occurs.
#### System Call Examples
```c
int
open (const char *file) {
	return syscall (SYS_OPEN, file);
}
```

