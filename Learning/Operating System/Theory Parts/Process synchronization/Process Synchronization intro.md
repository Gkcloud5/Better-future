#### Source:
[GFG](https://www.geeksforgeeks.org/introduction-of-process-synchronization/)
[JTP](https://www.javatpoint.com/os-process-synchronization-introduction)
[YT](https://www.youtube.com/watch?v=ph2awKa8r5Y&list=PLBlnK6fEyqRjDf_dmCEXgl6XjVKDDj0M2)


#### What is Process Synchronization in OS?

* When two or more process cooperates with each other, their order of execution must be preserved otherwise there can be conflicts in their execution and inappropriate outputs can be produces.
* Coordinating the execution of processes so that no two processes access the same shared resources and data is known as process synchronization.
* Procedure involved in preserving the appropriate order of execution of cooperative process is known as process synchronization.
* The need for process synchronization arises because multiple processes or threads running concurrently may share common resources, such as memory, files, devices or other system entities. without proper synchronization, simultaneous access to shared resources can lead to various problems
	* Race conditions
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

   