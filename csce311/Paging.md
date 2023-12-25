- Paging splits up address space into fixed-sized unit called a page
	- [[Segmentation]]: variable size of logical segments(code, stack, heap, etc.)
- With paging, physical memory is also split into some number of pages called a page frame
- Page table
- Main method to implement [[Memory Virtualization]]
- A page is dirty if it has been modified
	- Changes must be written to disk

##### Advantages of Paging
- Flexibility: Supporting the abstraction of address space effectively
	- Don't need assumption how heap and stack grow and are used
- Simplicity: Ease of free-space management
	- The page in address space and the page frame are the same size
	- Easy to allocate and keep a free list

##### Address Translation
- Two components in the virtual address
	- VPN
		- Virtual Page Number
	- Offset
		- Offset within the page

### Approaches to Paging
##### Hybrid Approach: Paging and Segments
- Combining [[Segmentation]] and Paging 
- [[Page Table]] for each Segment
	- In the page table, valid bits tell us whether or not we can use the memory
- Problems:
	- If we have a large but sparsely used heap, we can still end up with a lot of page table wasted
	- Causes External [[Fragmentation]] to arise again

##### Multilevel Paging 
- Multilevel paging is slower than single level paging
	- The [[TLB]] helps mitigate this loss in performance 
	- [[TLB]] misses are more severe
- The main advantage of multi-level paging is that we don't have to allocate all of this memory
	- We can allocate it as we need it
- Valid bits tell us what we actually need to allocate

![[two_level_paging_diagram.png]]

##### Inverted Page Table
- Keeping a single page table that has an entry for each physical page of the system
- The entry tells us which process is using this page, and which virtual page of that process maps to this physical page.
- Uses Hashing to check each frame for the VPN (I have no idea what this means)
- Advantages:
	- Saves memory
	- Performant
	