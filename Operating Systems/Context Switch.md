A low-level piece of assembly code
- Save a few register values for the current [[Process]] onto its kernel stack
	- General purpose registers
	- PC
	- Kernel stack pointer
- Restore a few for the soon-to-be-executing process from its kernel stack
- Switch to the kernel stack for the soon-to-be-executing process