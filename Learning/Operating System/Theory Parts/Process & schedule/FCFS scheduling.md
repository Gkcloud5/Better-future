#### Source:
[GFG](https://www.geeksforgeeks.org/program-for-fcfs-cpu-scheduling-set-1/)
[JTP](https://www.javatpoint.com/os-fcfs-scheduling)
[YT](https://www.youtube.com/watch?v=GS6yIngO4eg&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=22)


#### About FCFS scheduling:

* First come first serve
* It is a scheduling algorithm used by OS to allocate CPU time to processes.
* In FCFS scheduling, the OS simply execute the processes in the order they arrive, without considering any other factors such as process priority or resource requirement.
* It's not most efficient algorithm, if a CPU-bound process arrives first and uses the CPU for long time, then other processes may have to wait a long time before they can get a chance to use the CPU.


![[Pasted image 20230509170318.png]]

* It is a non-preemptive scheduling

#### Convoy effect:

* The convoy effect refers to a phenomenon where a long-running process holds up other shorter processes that arrived after it. this happens because the shorter processes have to wait for the long-running process to finish executing before they can start running on the CPU.
* 