#### Source:
[YT](https://www.youtube.com/watch?v=j0IqYWyBAKE&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=53)

#### About Paging:

* It is a example for non-contiguous memory 
	* Here available memory blocks are no need to have in order.

![[Pasted image 20230522122119.png]]


* In paging, 
	* the process is divided into no.of partitions called pages
		* size of a each page must be same.
	* Here main memory is also divided into no.of partitions called frame.
		* Size of each frame must be same
	* Page size and frame size must be equal.
	* Whenever CPU need to execute a process
		* Pages from the secondary memory is assigned to frames in main memory
	* Page table, 
		* Here page no as a input and produces frame number as a output.
		![[Pasted image 20230522124214.png]]

![[Pasted image 20230522124327.png]]

#### Paging Hardware:

* In order to execute any instruction CPU will create a logical address for a corresponding instruction.
* Logical address mainly divided into two parts
	* p --> Page number
	* d --> page offset --> displacement.
		* d --> Location of a page
* then page number given input to the page table.
	* Page table accepts a page number as input
	* and produce frame number as a output --> f
* Combine frame number with page offset then it give a physical address of the main memory.

![[Pasted image 20230522133621.png]]

