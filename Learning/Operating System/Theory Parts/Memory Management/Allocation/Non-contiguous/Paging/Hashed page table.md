#### Source:
[YT](https://www.youtube.com/watch?v=NyWcVoKjDu4&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=58)

* If we want to store lacks of entries inside a page table then we using hashed page table
	* Hashing provide function to locate a page table information.
* CPU produces logical address
	* P and D
* P will be given input to the hash function
	* It produces hash value that mapped to hash table
		* Each entry in hash table contain linked list, ignorer to maintain collision
* In linked list, each element have field
	* 1st field --> page number
	* 2nd field --> frame number
	* 3rd field --> address
		* If we have one node then address field is null
		* If we have 2nd node then address field value is address of 2nd node.

![[Pasted image 20230523212807.png]]

