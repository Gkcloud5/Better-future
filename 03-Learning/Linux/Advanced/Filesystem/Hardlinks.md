#### Source:
[LJ](https://linuxjourney.com/lesson/symlinks)

```
#create a hardlink
ln myfile2 myhardlink

93401 -rw-rw-r-- 2 pete pete 8 Jan 21 21:36 myfile2  
93402 -rw-rw-r-- 1 pete pete 8 Jan 21 21:36 myfile3 
93403 lrwxrwxrwx 1 pete pete 6 Jan 21 21:39 myfilelink -> myfile
93401 -rw-rw-r-- 2 pete pete 8 Jan 21 21:36 myhardlink
```

* It is also same as symlink but this is not shortcut
* Here hardlink file also connected to a inode so if you made any changes in any of file it will change modification to both files.
* But if i deleted any one of file then another file still there.
* Link count is the number of hardlinks that an inode has