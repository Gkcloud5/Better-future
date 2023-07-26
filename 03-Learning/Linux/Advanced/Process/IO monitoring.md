---
creation date: 2023-06-05 23:03
modification date: Monday 5th June 2023 23:03:56
tag: 
---

#### Source:
[LJ](https://linuxjourney.com/lesson/io-monitoring)

--------------------------------------

#### Explanation about it:

* Monitor CPU usage

```
iostat
```

![[Pasted image 20230605231441.png]]

* nice value is priority value assigned to a process.
* the nice value, also known as the niceness level, determines the priority at which a process will be schedules for CPU execution.
* %user - show the percentage of CPU utilization that occurred while executing at the user level(application)
* %nice - show the percentage of CPU utilization that occurred while executing at the user level with nice priority.
* %system - show the percentage of CPU utilization that occurred while executing at the system level(kernel)
* %iowait - Show the percentage of time that the CPU were idle during which the system had an outstanding disk IO request.
* %steal - show the percentage of time spent in involuntary wait by the virtual CPU while the hypervisor was servicing another virtual processor.
* %idle - Show the percentage of time that the CPU or CPUs were idle and the system did not have an outstanding disk I/O request.

![[Pasted image 20230606151440.png]]