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
* In order to overcome above problems, we use **TLB** --> **Translation look aside buffer**
	* Faster, special cache
	* it stores large amount of data
	* information stored here tag
		* Key and value format
	* In page table out of 100 address we will access repeatedly 10 address those are added in TLB for quick access.

![[Pasted image 20230522155051.png]]


#### [[Types of page table]]

