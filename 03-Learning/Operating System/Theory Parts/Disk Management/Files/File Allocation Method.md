#### Source:
[YT](https://www.youtube.com/watch?v=gK6L3v1b8AM&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=85)

* Generally files are stored in secondary storage device.
* File allocation method OS to allow hard disk space for a files
	* So that hard disk space can be used in effective manner.
	* As well as files can accessed faster manner.
* Types:
	* Contiguous allocation
	* Linked allocation
	* Indexed allocation

##### Contiguous allocation:

* In this approach a set of continues block will be allocated for a file

![[Pasted image 20230527143934.png]]

* File allocation table contain each and every file that is stored in secondary storage

![[Pasted image 20230527144040.png]]

* It is simply to implement.
* It is difficult to find our contiguous block.
* It have external fragmentation

#### Linked Allocation:

* It is based upon linked list.
* We have a collection of blocks, where we can have a pointer field so that one block pointer can contain next block address.

![[Pasted image 20230527150004.png]]

* File allocation table can have start and end block numbers
* Here no external fragmentation
* Here each block have some memory for pointer. 

#### Indexed Allocation:

 ![[Pasted image 20230527150312.png]]

* index contains all the blocks that related to file
* It supports both sequential and direct address
* here no external fragmentation.