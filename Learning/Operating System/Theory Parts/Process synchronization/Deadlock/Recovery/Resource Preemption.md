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
	* Minimum disruptio