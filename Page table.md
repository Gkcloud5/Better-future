#### Source:
[YT](https://www.youtube.com/watch?v=j0IqYWyBAKE&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=54)

* Here we are going to see where OS need to store page table
	* If we store page table inside a register, it's expensive and size of register is very low
		* Data assessable is very fast
	* Page table inside a memory
		* We required two memory access
			* For accessing page table --> logical address
			* For accessing the main memory --> physical address
		* We need 2 memory access for every single instruction, it's really hard to implement.
* In order to access a page table