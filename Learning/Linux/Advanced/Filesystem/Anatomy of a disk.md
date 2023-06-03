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

* Disks