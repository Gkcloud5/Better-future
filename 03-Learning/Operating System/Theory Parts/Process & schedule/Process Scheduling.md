#### Source:
[JTP](https://www.javatpoint.com/os-process-schedulers)
[YT](https://www.youtube.com/watch?v=K-Q85-gRmaA&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=10)

#### Why we need CPU scheduling:

* It decides which program must get into the the job queue.
* From the job queue. the job processor selects process and loads them into the memory for execution. 
* the main aim of the job scheduler is to maintain a good degree of multiprogramming.


#### About scheduling queue:

* Scheduling decides which process are going to execute next.
* In multiprogramming system multiple process are resides in main memory.
* Main goal is utilize CPU usage effective manner

#### Types:

##### 1. Long-term scheduler:

* Job scheduler
* It loads a process from secondary memory to main memory.
* In secondary memory we have a job queue it contains list of all the process which are in system.
* Ready queue resides in main memory.
* Long term scheduler mainly controls the degree of multiprogramming. the purpose of long term scheduler is to choose a perfect mix of IO bound and CPU bound processes among the jobs present in the pool.

##### 2. Short-term scheduler:

* It picks a process from ready queue and allocate CPU to that process.
* Other name is CPU scheduler
* A scheduling algorithm is used to select which job is going to be dispatched for the execution.

##### 3. Medium-term scheduler:

* It is used to while implementing swapping concept.
	* When CPU is executing one process if it receive interrupt then OS will transfer executing process to secondary memory.
* It is responsible for suspending and resuming the process.