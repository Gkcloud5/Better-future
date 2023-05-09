#### Source:
[JTP](https://www.javatpoint.com/os-srtf-scheduling-algorithm)
[YT](https://www.youtube.com/watch?v=Tcuyr91Y_Ro&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=24)

#### What is SRTF and why we need it?

* Shortest remaining time first scheduling algorithm
* It is a preemptive scheduling algorithm
* In SRTF, the scheduler selects the process with the shortest burs time to execute next
	* If a new process arrives with a shorter remaining burst time than the currently executing process, the scheduler preempts the running process and schedules the new process.
* It also have same drawback like SJF, starvation for long burst time process.