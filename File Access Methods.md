#### Source:
[YT](https://www.youtube.com/watch?v=0vno0Ra0wEg&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=77)
[JTP](https://www.javatpoint.com/os-file-access-methods)


* A file is a collection of related information which are stored in secondary storage.
* In order to access a data in file, OS have 3 options
	* Sequential access
	* Direct access (or) relative access
	* indexed sequential access

#### Sequential access:

* Most of the OS access the file sequentially.

![[Pasted image 20230526124237.png]]

* In sequential access, the OS read the file word by word. A pointer is maintained which initially points to the base address of the file.
	* If user wants to read first word of the file then the pointer provides that word to the user and increases its value by 1 word. this process continues till the end of the file.
* Modern way system provide the concept of 
	* Direct access
	* Indexed access
	* But most used method is sequential access
* Let consider, our file has 100 records, currently we are at 50th record now we want to access 75th record
	* we are using sequential access so if we want to access 75th record then access 51, 52, 53, .., 74 record to achieve 75th record.
	* not able to access record directly.
	* It takes more number of time in order to access a record

#### Direct access:

* By using this method we can access a record directly.
* Let consider file contain 100 instru