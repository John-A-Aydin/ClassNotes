- Page Tables hold the memory addresses of every page for a [[Process]] in [[Paging]]
- Page Tables can get awfully large
	- 32-bit address space with KB pages, 20 bits for VPN
		- Page offset for 4KB page: 20 bits
- Page tables for each process are stored in memory

##### What is the Page Table
- The page table is a data structure that is used to map the virtual address to physical address.
	- Simplest form: a linear page table, an array
- The OS indexes the array by VPN, and looks up the page-table entry

##### Common Flags of Page Table Entry
- **Valid Bit:** Indicating whether the particular translation is valid.
- **Protection Bit:** Indicating whether the page could be read from, written to, or executed from
- **Present Bit:** Indicating whether this page is in physical memory or on disk(swapped out)
- **Dirty Bit:** Indicating whether the page has been modified since it was brought into memory
- **Reference Bit(Accessed Bit):** Indicating that a page has been accessed

### Linear Table

We usually have one page table for every process in the system
- Assume that 32 bit address space with 4 KB pages and 4 byte page table entry 4KB
	- Page table will be too big and consume too much memory
- To get a smaller page table we can just make larger pages