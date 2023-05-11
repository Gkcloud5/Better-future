#### Source:
[GFG](https://www.geeksforgeeks.org/introduction-of-process-synchronization/)
[JTP](https://www.javatpoint.com/os-process-synchronization-introduction)

#### What is Process Synchronization in OS?

* When two or more process cooperates with each other, their order of execution must be preserved otherwise there can be conflicts in their execution and inappropriate outputs can be produces.
* Procedure involved in preserving the appropriate order of execution of cooperative process is known as process synchronization.
* The need for process synchronization arises because multiple processes or threads running concurrently may share common resources, such as memory, files, devices or other system entities. without proper synchronization, simultaneous access to shared resources can lead to various problems
	* Race conditions
	* Data corruption
	* Deadlock
	* Livelock

#### Some Process synchronization mechanism:

* [[Mutex]]
* [[Semaphores]]
* [[condition variable]]