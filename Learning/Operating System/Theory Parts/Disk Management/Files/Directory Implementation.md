#### Source:
[YT](https://www.youtube.com/watch?v=t8Rs9AbqHUc&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=83)
[JTP](https://www.javatpoint.com/os-directory-implementation)


*  There is the number of algorithm by using which, the directories can be implemented.
* However, the selection of an appropriate directory implementation algorithm may significantly affect the performance of the system
* Directory implementation algorithms are classified according to the data structure they are using
* Two algorithms
	* Linear List
	* Hash Table

#### Linear list:

* All the files in directory are maintained as single lined list.
* Each file contains the pointers to the data blocks which are assigned to it and the next file in the directory.

![[Pasted image 20230526200003.png]]

##### Characteristics:

* When a new file is created, then the entire list is checked whether the new file name is matching to a existing file name or not. 
* in case, it doesn't exit, the file can be created at the beginning or at the end.
* The list needs to be traversed