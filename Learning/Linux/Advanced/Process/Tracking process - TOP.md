---
creation date: 2023-06-05 21:12
modification date: Monday 5th June 2023 21:12:21
tag: #Process
---

#### Source:
[LJ](https://linuxjourney.com/lesson/tracking-processes-top)

--------------------------------------

#### Explanation about it:

* By using `top` command we can read and analyze the resource utilization on your system.
* top command provide real time view of the system utilization.

```
top - 18:06:26 up 6 days,  4:07,  2 users,  load average: 0.92, 0.62, 0.59
Tasks: 389 total,   1 running, 387 sleeping,   0 stopped,   1 zombie 
%Cpu(s):  1.8 us,  0.4 sy,  0.0 ni, 97.6 id,  0.1 wa,  0.0 hi,  0.0 si,  0.0 st 
KiB Mem:  32870888 total, 27467976 used,  5402912 free,   518808 buffers
KiB Swap: 33480700 total,    39892 used, 33440808 free. 19454152 cached Mem

  PID  USER      PR  NI    VIRT    RES    SHR S  %CPU %MEM     TIME+ COMMAND           6675 patty    20   0 1731472 520960  30876 S   8.3  1.6 160:24.79 chrome             6926 patty    20   0  935888 163456  25576 S   4.3  0.5   5:28.13 chrome
```

##### 1st line:
* Show current time
* How long the system has been running
* How many users are currently logged on
* System load average (more to come)

##### 2nd line:
* Tasks that are running, sleeping and stopped and zombied.


##### 3rd line:
* CPU information
* us: User CPU time - percentage of CPU time spent running users processes that are not niced.
* sy: System CPU time - percentage of CPU time spent running the kernel processes