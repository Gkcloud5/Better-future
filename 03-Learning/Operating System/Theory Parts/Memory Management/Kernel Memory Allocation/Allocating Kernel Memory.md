#### Source:
[YT](https://www.youtube.com/watch?v=sKWSk0o-TxE&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=72)

* Usually, OS allocating user level process by using two approach
	* Contiguous memory allocation
	* Non-contiguous memory allocation
* Main memory divided into two parts
	* 1st part is OS
	* 2nd part is User programs
* in first part they have driver info
* Every process have
	* Process descriptors
	* File object
	* semaphore
		* All these stored in kernel
	* In order to assign memory to kernel object, we have 2 approach
		* [[Buddy System]]
		* [[Slab Allocation]]