#### Source:
[LJ](https://linuxjourney.com/lesson/anatomy-of-a-disk)

* Hard disks can be subdivided into partitions.
* Partitions are extremely useful for separating data and if you need certain file system.

#### Partition table:

* Every disk will have a partition table, this table tells the system how disk is partitioned.
* This table tells you where partitions begin and end, which partitions are bootable, what sectors of the disk are allocated to what partition.
* Two main partition table schemes used
	* Master Boot Record
	* GUID Partition Table.

#### Partition:

* Disks are comprised of partitions that help us organize our data. 
* You can have multiple partitions on a disk and they can't overlap each other.
* If space not allocated in a partition, then it is known as free space.
* The types of partitions depend on your partition table

##### MBR:

* Traditional partition table, was used as standard.
* Can have primary, extended and logical partitions.
* MBR has a limit of four primary partitions.

##### GPT:

* GUID Partition Table, new standard for disk partitioning
* Has only one type of partition and you can make many of them
* Each partition has globally unique ID.
* Used mostly in conjunction with UEFI based booting.

#### File system structure:

* File system is an organized and collection of files and directories.

##### Boot Block:

* This is located in the first few sectors of the filesystem, and it's not really used by the file system.
* It contains information used to boot the OS
* Only one boot block is needed by the OS.

##### Super Block:

* This is single block it comes after the boot block.
* It contains information about the filesystem, such as size of the inode table, logical blocks and the size of the filesystem.

##### Inode table:

* This is a database that manages our files.
* Each file or directory has a unique entry in the inode table and it has various infomation about the files.

