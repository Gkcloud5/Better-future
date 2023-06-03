#### Source:
[LJ](https://linuxjourney.com/lesson/symlinks)


* Symbolic link is a same as windows shortcut feature.
* Symlink allow us to link to another file by its filename.
* Hardlink is actually another file with a link to a inode.

```
  
pete@icebox:~/Desktop$ echo 'myfile2' > myfile2
  
pete@icebox:~/Desktop$ echo 'myfile3' > myfile3

pete@icebox:~/Desktop$ ln -s myfile myfilelink
  
pete@icebox:~/Desktop$ ls -li
  
total 12
  
  151 -rw-rw-r-- 1 pete pete 7 Jan 21 21:36 myfile
  
93401 -rw-rw-r-- 1 pete pete 8 Jan 21 21:36 myfile2
  
93402 -rw-rw-r-- 1 pete pete 8 Jan 21 21:36 myfile3
  
93403 lrwxrwxrwx 1 pete pete 6 Jan 21 21:39 myfilelink -> myfile
```


* Symbolic links are denoted by ``-``
* When a modify a symlink then file also gets modified.
* Inode numbers are unique to filesystems
* 