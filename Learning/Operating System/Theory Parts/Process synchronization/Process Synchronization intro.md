#### Source:
[GFG](https://www.geeksforgeeks.org/introduction-of-process-synchronization/)
[JTP](https://www.javatpoint.com/os-process-synchronization-introduction)
[YT](https://www.youtube.com/watch?v=ph2awKa8r5Y&list=PLBlnK6fEyqRjDf_dmCEXgl6XjVKDDj0M2)


#### What is Process Synchronization in OS?

* When two or more process cooperates with each other, their order of execution must be preserved otherwise there can be conflicts in their execution and inappropriate outputs can be produces.
* Coordinating the execution of processes so that no two processes access the same shared resources and data is known as process synchronization.
* Procedure involved in preserving the appropriate order of execution of cooperative process is known as process synchronization.
* The need for process synchronization arises because multiple processes or threads running concurrently may share common resources, such as memory, files, devices or other system entities. without proper synchronization, simultaneous access to shared resources can lead to various problems
	* [[Race conditions]]
	* Data corruption
	* Deadlock
	* Livelock

![[Pasted image 20230512170240.png]]



#### Some Process synchronization mechanism:

* [[Mutex]]
* [[Semaphores]]
* [[condition variable]]
* [[Barriers]]
* [[Atomic Operations]]
* [[Critical sections]]
* [[Monitors]]

**Independent process:**
   The execution of one process does not affect the execution of other processes.

**Cooperative process:**
   * A process that can affect or be affected by other processes executing in the system
   * Process synchronization problem arises in the case of cooperative process also because resources shared in cooperative process.


#### Process synchronization becomes crucial for the following reasons:

##### Data Consistency:
* When multiple processes or threads access and modify shared data simultaneously, there is a risk of data corruption or inconsistent results.
* Following mechanism will help to solve this issue
	* Locks
	* Semaphores
	* Mutexes
	* Mutual exclusion
		* Allowing only one process or thread to access the shared resources at a time, it preventing race conditions and maintaining data consistency.

##### Resource Allocation:
* In many scenarios, multiple processes or threads may compete for limited resources, such as files, network connections, or hardware devices.
* Process synchronization techniques help manage resource allocation by allowing processes or threads to request and release resources in an organized way.

##### Interprocess communication:
* Process often need to communicate and exchange data with each other. 
* Synchronization mechanisms, such as
	* Message queues
	* shared memory
	* condition variables
		* Above are helps to avoid busy-waiting or race conditions.

##### Avoid deadlocks:
* Deadlock occurs when multiple processes or threads are waiting for each other to release resources, resulting in a situation where none of them can proceed.
* Resource allocation strategies will to solve this issue.

##### Timing and order control:
* Synchronization mechanism also enable timing and order control in concurrent processes or threads.
* Example, Barriers can be used to ensure that group of processes or threads reaches particular point in their execution before processing.


#### Problems:

1. [[Bounded Buffer problem]]
2. [[Readers writers problem]]

