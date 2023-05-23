#### Source:
[YT](https://www.youtube.com/watch?v=H7cJsF79iew&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=55)


#### About segmentation:

* It is mainly used to maintain modular structure of program.
* It's used to divide physical memory into logical segments.
	* Each segment can be used by a different process or thread.
	* Each segment can have its own permission.
* This allows the OS to protect different parts of memory from each other.
* And to prevent one process from accidentally or maliciously overwriting process's memory.
* Major drawback of paging is a module may resides in different pages of process

 ![[Pasted image 20230523140039.png]]

* In paging, process are stored in page table randomly, does not have any modular structure.
* Segmentation is non-contiguous memory
	* Segment means collection of statements.
* Given process divided into number of partitions but here size of partition is similar to a size of segment.
	* Main memory also divided into number of partitions, size of partition is similar to a size of segment.
* CPU generates logical address
	* divided into two parts
		* 1st part is segment number
		* 2nd part is offset
* Segment