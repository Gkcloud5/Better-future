#### Source:
[JTP](https://www.javatpoint.com/os-preemptive-priority-scheduling)
[GFG](https://www.geeksforgeeks.org/program-for-preemptive-priority-cpu-scheduling/)
[YT](https://www.youtube.com/watch?v=wldjV-wVvhg&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=25)

#### What is preemptive scheduling and why we need it?

* Preemptive priority scheduling algorithm in which the CPU can be taken away from a running process if a higher-priority process becomes ready for execution.
* In here, at the time of arrival of a process in the ready queue, its priority is compared with the priority of other processes present in the ready queue as well as with the one which is being executed by the CPU at that point of time, the one with highest priority among all the available processes will be given the CPU next.

![[Pasted image 20230510165518.png]]

