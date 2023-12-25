Swapping policies are used in [[Cache Management]] for [[Paging|paging]] to keep relevant pages in the cache 
### The Optimal Replacement Policy
- Leads to the fewest number of misses overall
	- Replace the page that will be accessed furthest in the future
	- Result in the fewest possible cache misses
- Serves only as a comparison point, to know how close we are to perfect

### The Simple Policy: FIFO
- Pages were placed in a queue when they enter the system.
- When a replacement occurs, the page on the tail of the queue(the “First-in” pages) is evicted.
	- It is simple to implement, but can’t determine the importance of blocks.
	- This algo sucks butt

### Another Simple Policy: Random 
- Picks a random page to replace under memory pressure.
	- It doesn’t really try to be too intelligent in picking which blocks to evict.
	- Random does depends entirely upon how lucky Random gets in its choice.

## Using History
- Learn on the past and use history
	- Recency (LRU)
		- The more recently a page has been accessed, the more likely it will be accessed again
	- Frequency (LFU)
		- If a page has been accessed many times, It should not be replaced as it clearly has some value
- Replace the least-recently-used page. 

##### Workload Example : The No-Locality Workload
- Each reference is to a random  page within the set of accessed pages.
	- Workload accesses 100 unique pages over time.
	- Choosing the next page to refer to at random

##### Workload Example: The Looping Sequential
- Refer to 50 pages in sequence.
	- Starting at 0, then 1, … up to page 49, and then we Loop, repeating those accesses, for total of 10,000 accesses to 50 unique pages.
	- LRU and FIFO have terrible performance.
	- Random excels here
	