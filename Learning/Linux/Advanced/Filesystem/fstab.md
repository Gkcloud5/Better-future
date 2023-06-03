#### Source:
[LJ](https://linuxjourney.com/lesson/etc-fstab-file-system-table)

* it contains permanent list of filesystems that are mounted.

```
cat /etc/fstab
UUID=130b882f-7d79-436d-a096-1e594c92bb76 /    ext4 relatime,errors=remount-ro 0  1
  
UUID=78d203a0-7c18-49bd-9e07-54f44cdb5726 /home xfs     relatime        0       2
  
UUID=22c3d34b-467e-467c-b44d-f03803c2c526 none  swap    sw              0       0
```

* UUID -- Device identifier
* Mount Point --> Directory the filesystem is mounted to
* Filesystem type
* Options --> Other mount options, man page will help to know more
* Dump --> 0 is default, used by the dump utility to decide when to make a backup
* Pass --> used by fsck to decide what order filesystems should be checked. if the value is 0, it will not be checked

