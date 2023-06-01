#### Source:
[YT](https://www.youtube.com/watch?v=hDBFSQRHPAU&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=86)

* After allocating a memory for a file in hard disk, it have some free space so how OS is managing that free space.
* When file is deleted there is some free the OS how manage that free space.
* 4 Approach:
	* Bit-vector
	* Linked-list
	* Grouping
	* Counting

#### Bit-Vector:

* Hard disk contain collection of block.
* Here each block is represented by bit.
	* If bit 0 then it's occupied
	* If bit is 1 then it's free

 ![[Pasted image 20230527173802.png]]

* It is very easy to implement.

#### Linked-List:

![[Pasted image 20230527174036.png]]

* Here is no wastage of space.
* Each block should need contain pointer, it take some extra space in memory


#### Grouping:

* Stored address of n-1 free blocks in 1st free block.

#### Counting:

* In addition to next free block pointer, keep a pointer saying how many blocks are continuously free after a free block.