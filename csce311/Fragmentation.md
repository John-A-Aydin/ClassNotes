
##### External Fragmentation:
- Little holes of free space in physical memory that is too small for allocation a segment
	- There is 24KB free, but not in one contiguous segment.
	- The OS cannot satisfy the 20KB request

##### Internal Fragmentation:
- Space of unused memory between stack and heap
### Ways to fix fragmentation
##### Compaction:
- Rearranging the existing segments in physical memory
	- Compaction is costly
		- Stop running process.
		- Copy data to somewhere.
		- Change segment register value

##### [[Paging]]