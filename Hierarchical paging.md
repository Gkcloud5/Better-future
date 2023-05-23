#### Source:
[YT](https://www.youtube.com/watch?v=Sa3Z-aFINuE&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=56)

* Size of logical address is 32-bit.
* Size of a page is 4KB.
	* 2^12
* Here page table divided into two parts
	* Page number --> 2^20 --> 20bit
	* Offset --> 2^12 --> 12 bit
* totally we can store 2^20 page numbers, it's more than 10lakh
* Here, instead of storing a entire page table in one table, OS splitting multiple page tables
* Outer page table accept input as page number and produce offset output 
	* Offset can be provided index of another page table.
		* This page table product frame number as output
* offset and frame number combined, it gives exact physical address of main memory
 
