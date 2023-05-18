#### Source:
[YT](https://www.youtube.com/watch?v=23xp51q2LP0&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=39)


#### Necessary conditions for deadlock:

*  4 Condition will lead to make deadlock
	* Mutual exclusion
	* Hold and wait
	* No preemption
	* Circular wait
* If above 4 conditions occurs simultaneously in a system then deadlock will occur

##### Mutual exclusion:

* A process can use only one resources at a time.
* All the resources are non sharable default.
* Sharing a single resources to multiple process will lead data confusion
* we need to eliminate mutual exclusion inorder to avoid deadlock.

##### Hold and Wait:

* A process is holding some resources and waiting for additional resources but incase additional resource is allocated to some other process it will make process to wait until additional process complete.
	* During this time process holding resources is completely waste.

![[Pasted image 20230518195740.png]]

##### No preemption:

* Non preemptive means CPU cannot stop executing process
* In deadlock scenarion CPU should stop process so we shol