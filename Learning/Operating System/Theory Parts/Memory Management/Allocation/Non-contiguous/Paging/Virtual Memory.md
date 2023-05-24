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

![[Pasted image 20230524122442.png]]


* CPU executing program A, it completed program A then page of program A moved from main memory to secondary memory.
	* This is known as swap-out
* CPU is ready for executing program, then OS swap pages from secondary memory to main memory.
	* This process is known as swap-in.


##### Page table when some pages not in main memory:

* Totally process have 5 pages here.
* page table
	* Input is process page number
	* It produce frame number as output
* In page table, valid bit or invalid bit represent page is allocated in main memory or not.


![[Pasted image 20230524123737.png]]


#### Page fault:

* When CPU need to execute a page it checks whether page is allocated in main memory or not.
* If the page is available in main memory then there is no problem
* If page is not available in main memory then it's called **page fault**

##### Steps in handling page fault:


![[Pasted image 20230524125354.png]]

##### Step 1:

* CPU checks whether pages is present in page table or not.
	* I is invalid it specify page is not present in main memory.

##### Step2:

* Here page is not present in main memory then interrupt call trap to the OS

##### Step 3:

* OS checks where that page is present in seconda
