#### Source:
[YT](https://www.youtube.com/watch?v=bOFDyPKTgXM&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=61)


* Whenever CPU need to execute a page
	* It check page is present in main memory or not
		* If the page is not present in main memory then **page fault** will occur
			* Whenever page fault occurs then OS loads a page from secondary to main memory
				* At that time main memory is filled then we need to replace any of page from main memory and need to allocate those space to a secondary memory page.
* Which page should replace that decide based on page replacement algorithm.
* 