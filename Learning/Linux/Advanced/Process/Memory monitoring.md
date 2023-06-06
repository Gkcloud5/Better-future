---
creation date: 2023-06-06 15:26
modification date: Tuesday 6th June 2023 15:26:37
tag: 
---

#### Source:
[LJ](https://linuxjourney.com/lesson/memory-monitoring)

--------------------------------------

#### Explanation about it:

* we can monitor memory usage by using following command

```
vmstat
```

```
pete@icebox:~$ vmstat
  
procs -----------memory---------- ---swap-- -----io---- -system-- ------cpu----- 
 r  b   swpd   free   buff  cache   si   so    bi    bo   in   cs us sy id wa st 
 1  0      0 396528  38816 384036    0    0     4     2   38   79  0  0 99  0  0
```


##### Procs:

* r- Number of process for run time.
* b - number of processes in uninterruptible sleep

##### Memory:

* swpd - Amount of virtual memory used
* free - Amount of free memory
* buff - Amount of memory used as buffers [[Buffering]]
* cache - Amount of memory used as cache
	* cache is high speed storage area that used to store frequently accessed data or instruction for faster access.

##### swap:

* si - amount of memory swapped in from disk
* so - amount of memory swapped out to disk

##### Interrupts:

* 