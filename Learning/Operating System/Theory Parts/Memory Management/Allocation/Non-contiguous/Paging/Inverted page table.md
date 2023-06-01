#### Source:
[YT](https://www.youtube.com/watch?v=arIuMrC06fA&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=59)

* Generally each process have its own page table.
* Let consider process p1, it has 100 pages
	* Assume only 10 pages are available in main memory
* Process page table contains all the information, 100 instructions.
* Problem is,
	* Size of process is 100pages but main memory only have 10 pages
	* Here page tables contain all the instruction even though it does not resides in main memory.
* In this type, number of available page table instruction is depends upon main memory pages count.
	* If main memory contains 100 pages then inverted page table also have a 100pages


![[Pasted image 20230523214636.png]]

