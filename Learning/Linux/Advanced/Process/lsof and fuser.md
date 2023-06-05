---
creation date: 2023-06-05 22:22
modification date: Monday 5th June 2023 22:22:12
tag: 
---

#### Source:
[LJ](https://linuxjourney.com/lesson/tracking-processes-lsof-fuser)

--------------------------------------

#### Explanation about it:

* Some time when we unmount a device we get following error, "Device or Resource Busy". we can use following tool to know which file is a reason for this error

##### lsof:

* list open files
* it shows list of all the open files and their associated process.

```
lsof
  
COMMAND    PID  USER   FD   TYPE DEVICE SIZE/OFF NODE NAME 

lxsession 1491 pete  cwd    DIR    8,6     4096  131 .  
update-no 1796 pete  cwd    DIR    8,6     4096  131 . 
nm-applet 1804 pete  cwd    DIR    8,6     4096  131 . 
indicator 1809 pete  cwd    DIR    8,6     4096  131 . 
xterm     2205 pete  cwd    DIR    8,6     4096  131 . 
bash      2207 pete  cwd    DIR    8,6     4096  131 . 
lsof      5914 pete  cwd    DIR    8,6     4096  131 .
lsof      5915 pete  cwd    DIR    8,6     4096  131 .
```


##### fuser:

* file user
* This will show you information about the process that is using the file or the file user

```
fuser -v
```

![[Pasted image 20230605222537.png]]

