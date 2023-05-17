#### Source:
[YT](https://www.youtube.com/watch?v=kOYTmxKpIms&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=47)


**Preemption means releasing a resources**

#### 3 issues needs to consider while preempting a resources:

##### 1. Selecting a Victim:

* Which resources we have to select to release from the process.
* If process have 10 resources then need to select which resource need to release

##### 2. Rollback:

* What should we have to do in which resources is released
* Simply we have to start execution from beginning

##### 3. Starvation:

* There may be possibility for single process resources may be released, so in this situation some process waiting for abort process.


#### Overview of How resource preemption works:

##### 1. Deadlock detection:

* First, a deadlock detection algorithm will help to identify a deadlock

##### 2. Resource selection:

* Once a deadlock is detected, a decision must be made regarding which processes to target for resource preemption.
* Various strategies can be used to select the process
	* Minimum disruption
	* process with lower priority
	* Process that has made the least progress

##### 3. Resource reclamation:

* After selecting the process, the resources held by these processes are forcefully reclaimed.
* This will release the resource and making them available for allocation to other process.

##### 4. Process suspension:

* When resources are preempted from a process, the process may enter a suspended state.
* State of process is saved, it wait to get resources that it need

##### 5. Resource allocation:

* Resources that were involved in the deadlock are now allocated to other waiting processes in order to break the deadlock.

##### 6. Deadlock resolution:

* After resource al