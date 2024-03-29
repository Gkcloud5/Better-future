#### Source:
[LJ](https://linuxjourney.com/lesson/inodes)

* How our filesystem is comprised of all our actual files and a database that manages these files? the database is known as the inode table


#### What is an inode?

* An inode(index node) is an entry in this table and there is one for every file. it describes everything about the file, such as
	* File type - regular file, directory and character device
	* Owner
	* Group
	* Access permission
	* Timestmps
	* Number of hardlink to the file
	* Size of the file
	* Number of blocks allocated to the file
	* Pointers to the data block
* Basically, inode stores everything about the file, except the file name and the file itself!

#### When are inodes created?

* When a filesystem is created, space for inodes is allocated as well.
* There are algorithms that take place to determine a size of inode.

#### Inode information:

```
ls -li
```

* Inodes are identified by numbers, when a file gets created it is assigned an inode number.
* Number is assigned in sequential order.

```
stat ~/Desktop/
```


#### How do inodes locate files?

* Inodes point to the actual data blocks of your files.
* In a typical filesystem, each inode contains 15 pointers, the first 12 pointers point directly to the data blocks.
* the 13 the pointers point to a block containing pointers to more blocks.
* the 14th pointer points to another nested block of pointers. 
* and 15th pointer points yet again to another block of pointers.