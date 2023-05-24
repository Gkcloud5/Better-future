#### Source:
[YT](https://www.youtube.com/watch?v=bOFDyPKTgXM&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=61)


* Whenever CPU need to execute a page
	* It check page is present in main memory or not
		* If the page is not present in main memory then **page fault** will occur
			* Whenever page fault occurs then OS loads a page from secondary to main memory
				* At that time main memory is filled then we need to replace any of page from main memory and need to allocate those space to a secondary memory page.
* Which page should replace that decide based on page replacement algorithm.

#### Steps:

1.  We need to select a page from a main memory and need to swap it to secondary memory
	1. So we have 1 free space now.
2. We need to update swapped page status to invalid in page table.
3. We have swap in a page from secondary memory to main memory
4. Need to update newly swapped page status to valid bit.

![[Pasted image 20230524131027.png]]


#### Some algorithm:

[[FIFO page replacement]]

[[Belady's Anomaly - FIFO]]
