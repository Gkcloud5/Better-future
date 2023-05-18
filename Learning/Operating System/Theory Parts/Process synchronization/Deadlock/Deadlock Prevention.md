#### Source:
[YT](https://www.youtube.com/watch?v=GAde3Skbs8I&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=41)


#### About Deadlock prevention:

* Bestway to avoid deadlock is taking medicine before  the disease
	* During OS design takes necessary action to avoid deadlock.
* Necessary condition for deadlock
	* Mutual exclusion
	* Hold and wait
	* No Preemption
	* Circular wait
		* In order to avoid one or two condition, so that we will eliminate a deadlock.

##### Avoiding mutual exclusion:

* Ensure that resources cannot be simultaneously held by multiple processes.
* By allowing only one process to access a resource at a time, then condition of mutual exclusion is satisfied.

##### Avoiding Hold and Wait:

* Modify the system to ensure that a process must request and acquire all the resources it needs before execution starts.
	* This prevent  process from holding resource and waiting for another resources.

##### No Preemption:

* Allow resources to be preempted or forcibly taken away from processes if necessary.
* This means if one process holding a resources and request a additional resources, incase additional resources was allocated to some other process then this process will release resources.

##### Circular Wait:

*  Prevent the formation of circular chains of processes waiting for resources. 
* In order to avid this, we need to assign resources to process
