#### Source:
[GFG](https://www.geeksforgeeks.org/preemptive-and-non-preemptive-scheduling/)
[YT](https://www.youtube.com/watch?v=ProLx3vbhQs&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=20)

#### Preemptive scheduling:

##### What is preemptive scheduling:

* In preemptive scheduling algorithm used in OS where a running process can be interrupted and suspended by then OS to allow other high-priority processes to execute.
* It is designed to provide better responsiveness and fairness to different processes running in the system.
* One of the main reason for using preemptive scheduling is to ensure that high priority processes are executed in a timely manner.
* It is used when a process switches from running state to ready state or from the waiting state to ready state. the resources are allocated to the process for a limited amount of time and then taken away, and the process is again placed back in the ready queue.


#### Non-preemptive scheduling:

##### What is non-preemptive scheduling:

*  It is a scheduling algorithm used in OS where a running process cannot be interrupted or preempted by the OS until it has completed.
* The non-preemptive scheduling algorithm is designed to ensure that a process is not interrupted while its executing critical tasks or has acquired important system resources.
* In this scheduling, once the resources are allocated to a process, the process holds the CPU till it gets terminated or reaches a waiting state.
