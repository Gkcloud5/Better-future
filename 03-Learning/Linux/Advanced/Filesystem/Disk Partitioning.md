#### Source:
[LJ](https://linuxjourney.com/lesson/disk-partitioning)

* Tools help to create a partition
	* fdisk --> It does not support gpt
	* parted --> It support both MBR and GPT
	* gparted --> GUI version of parted
	* gdisk --> it does not MBR.

#### To check disk usage:

```
df -h
du -h
```

* df -h --> shows utilization of your currently mounted filesystems.
* du -h --> it shows disk usage of current directory you are in.