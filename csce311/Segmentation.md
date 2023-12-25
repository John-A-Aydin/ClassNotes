- A Segment is just a contiguous portion of the address space of a particular length
	- Logically-different segment: code, stack, heap
- Segments can be placed in different parts of the physical memory
	- Base and bounds exist per each segment

##### Address Translation

Code:
- physical address = offset + base
Heap:

##### Segmentation Fault or Violation
- If an illegal address such as 7KB which is beyond the end of heap is referenced, the OS occurs segmentation fault
	- The hardware detects that address is out of bounds

### Referring to Segment

##### Explicit Approach
- Chop up the address space into segments based on the top few bits of virtual address

##### Implicit Approach
- Does code simply call a load for all data accessed? No.
- How to identify instruction addresses?
	- Based off of PC (part of fetch)
- How to identify stack addresses?
	- Address modified from stack pointer
- How to identify heap addresses?
	- If previous two don’t apply, use heap segment.

### Problems with Segmentation

##### [[Fragmentation]]
- Since segments are continuous blocks of memory and processes need varying amounts of memory, segmentation can cause a lot of external fragmentation.