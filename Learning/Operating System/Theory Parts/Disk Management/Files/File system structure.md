#### Source:
[YT](https://www.youtube.com/watch?v=K7PVWaF7sX0&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=82)

* A file is a collection of related information
* Generally, file system stored in secondary storage device
* In order to perform operation in secondary storage, file system configured several layers

![[Pasted image 20230526193817.png]]

##### Application program:

* Program which is developed by a users is known as application program.

##### Logical file system:

* It check the above program is whether program is directory structure or not
* Logical block
* Physical block --> it specify exact number of block stored in secondary storage.

##### File organization module:

* It accepts logical block number as input and it perform mapping in order to find physical block of program.

##### Basic File system:

* Physical block is input for this.
* it give control to that block to IO control