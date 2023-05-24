#### Source:
[YT](https://www.youtube.com/watch?v=3CC7WOwDjac&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=60)

* CPU execute a process if it's resides in main memory only.
* Process is a collection of pages
* Each page is a collection of instruction
* If size of process is larger than size of a main memory.
	* Size of process is 10GB
	* Size of main memory is 4GB
		* Generally, not possible to store process to main memory because of process larger size.
			* By using **virtual memory** to solve this issue
* Virtual memory is implemented by using demand paging.
* Whenever there is a demand of a page then only OS will loads that page into main memory.

