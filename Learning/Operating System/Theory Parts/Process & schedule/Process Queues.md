#### Source:
[JTP](https://www.javatpoint.com/os-process-queues)
[YT](https://www.youtube.com/watch?v=iLC--q7O_KM&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=9)

#### Why we need process queue?

* In OS processes are often managed using a process queue, which is a data structure that holds a list of processes waiting to be executed or waiting for particular event to occur.
* Some reasons:
	* Resource allocation
	* Synchronization
	* Priority management
	* Event management

![[Pasted image 20230507185421.png]]


#### Types of queue:

##### 1. Job queue:

* It contains list of all the process which are in system.
* Generally content of job queue will be stored in hard disk.
* Long term scheduler picks some of the jobs and put them in the primary memory.

##### 2. Ready queue:

*  It contains list of all the process which are waiting for execution by CPU.
* 