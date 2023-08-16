
### Source:

1. [PN](https://phoenixnap.com/kb/linux-commands-check-memory-usage)

## Commands:

* #### Using `cat`:

```
cat /proc/meminfo
```

* This is the file which have reports the amount of available and used memory.
* It contains real time system's memory
	* Buffer
	* Shared Memory

![[Pasted image 20230816180216.png]]

* #### `free` command:
```
free
```

![[Pasted image 20230816180347.png]]

* It display amount of physical and swap memory

![[Pasted image 20230816180706.png]]

* #### `vmstat` Command:

```
vmstat
```

![[Pasted image 20230816180856.png]]

* r        --> number of processes waiting for run time
* b       --> no.of processes in uninterruptible sleep
* swpd --> amount of virtual memory used
* free   --> amount of idle memory
* buff   --> the amount of memory used as buffers
* cache --> amount of memory used as cache
* si        --> Memory swapped in from disk (/s)
* so      --> Memory swapped to disk (/s)
* bi      --> Blocks received from a block device(blocks/s)
* bo     --> Blocks sent to a block device (blocks/s)
* in      --> no.of interrupts per second, including the clock
* cs      --> number of context switches per second
* us      --> time spent running non kernel code (user time, including nice time)
* sy      --> Time spent running kernel code (system code)
* id      --> time spend idle.
* wa     --> Time spent waiting for IO
* st       --> time stolen from virtual machine

* #### `top` Command:

```
top
```
* It used to check memory and CPU usage per process
*  It display following information
	* uptime
	* Average load
	* tasks running
	* no.of users loggedin
	* no.of CPU utilization
	* memory/swap system processes

![[Pasted image 20230816181958.png]]

