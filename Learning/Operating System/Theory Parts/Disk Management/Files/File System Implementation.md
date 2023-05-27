#### Source:
[YT](https://www.youtube.com/watch?v=t8Rs9AbqHUc&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=83)

* we use two types of structure
	* on-disk structure
	* In-memory structure

#### On-Disk structure:

* This structure maintained inside disk, that is nothing but secondary storage.

##### Boot Control Block:

* It contains information that is needed to boot.

##### Volume control block:

* It contains information about that partition or volume.
* Secondary storage each partition will have volume control block.
* Size of block, how many blocks are free information is stored here

##### Directory structure:

* It used to organize a files.

##### File control block:

* It contains information about a file
	* What type of file
	* Size of file
	* owner of file

![[Pasted image 20230527142443.png]]

#### In-Memory structure:


![[Pasted image 20230527142456.png]]

* This structure are maintained inside a main memory.

##### In-memory mount table:

* It contains information about mount point.

##### In-Memory directory s