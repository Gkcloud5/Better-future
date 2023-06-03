#### Source:
[LJ](https://linuxjourney.com/lesson/inodes)

* How our filesystem is comprised of all our actual files and a database that manages these files? the database is known as the inode table


#### What is an inode?

* An inode(index node) is an entry in this table and there is one for every file. it describes everything about the file, such as
	* File type - regular file, directory and character devu