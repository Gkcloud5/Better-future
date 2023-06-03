#### Source:
[LJ](https://linuxjourney.com/lesson/creating-filesystems)

```
sudo mkfs -t ext4 /dev/diskpart1
```

mkfs --> make filesystem
	* It allow us to specify the type of filesystem we want and where we want it.
* You only create a filesystem on a newly partitioned disk.


#### Mount and unmount:

* Before you can view the contents of your filesystem, you will have to mount it.

```
mount -t ext4 /dev/diskpart1 /directorypath
```

```
umount /directorypath
```

```
#To view UUID
blkid
```
