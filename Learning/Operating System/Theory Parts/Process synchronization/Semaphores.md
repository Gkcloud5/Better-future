#### Source:
[YT](https://www.youtube.com/watch?v=5y14WXehSU4&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=37)
[JTP](https://www.javatpoint.com/os-semaphore-introduction)
[GFG](https://www.geeksforgeeks.org/semaphores-in-process-synchronization/)

#### About semaphores:

* Semaphore is a integer variable that is shared by multiple processes.
* It is a synchronization mechanism used to coordinate the activities of multiple processes in a computer system.
* We can initially semaphore variable and we can accessed by 2 standard operations
	* Wait
	* Signal
* Semaphore is a simply an integer variable that is shared between threads. this variable is used to solve the critical section problem to achieve process synchronization in the multiprocessing environment.

![[Pasted image 20230515150227.png]]


#### Mutual exclusion implementation:

![[Pasted image 20230515150407.png]]

* Let consider two process p1 and p2.
* Critical section only shared memory accessed.
	* If one process is in critical section then no other process allowed in critical section until previous process completed.
* **Mutex** is a semaphore variable. it will make changes in wait and signal system call inorder to allow process in critical section
* Initially mutex value is 1
* wait(1) -->