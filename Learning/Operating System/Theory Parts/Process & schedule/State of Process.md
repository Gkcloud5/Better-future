#### Source:
[GFG](https://www.geeksforgeeks.org/states-of-a-process-in-operating-systems/)
[Yt-1](https://www.youtube.com/watch?v=SGxFMEZ-ypc&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=7)
[JT](https://www.javatpoint.com/os-process-states)


### Process state:

* Process means program during execution.

#### 1.New:

* When ever program is loaded into main memory by OS then process state will be **new** state.

#### 2.Ready:

* Here process is ready for execution, it is waiting for CPU to execute a program.
* Whenever a process is created, it directly enters in the ready state.
	* It waits for CPU to be assigned.

#### 3. Running:

* It means CPU executing a process, if one process is executing in CPU then that process status will be running state.
* Mostly process pick from ready state by scheduling algorithm.

#### 4. Waiting:

* A process while in running state, if it need some IO operation then process will move to waiting state.
* Once IO completed process will move to ready state.

#### 5. Terminated:

* If process completed all the operation then it will moved to terminated state from running.
* It will freeup a resources.
* All the context of the process(PCB) will be deleted and process will be terminated by the OS.

#### 6. Suspend ready:

* Here mostly process state change from ready state.
	* Process moved from secondary memory from main memory due to lack of the resources.
* If the main memory is full and higher priority process comes for the execution then OS need to make a room for the process in the main memory by throwing lower priority process out into the secondary memory.

#### 7. Suspend wait:

* Similar to suspend ready but used the process which was performing IO operation and lack of main memory caused them to move to secondary memory.
* When work is finished it may go to suspend ready.

### Operations on the process:

#### 1. Scheduler:

* It allocate process from ready to CPU that means change process state to running.

#### 2. Interrupt:

* whenever process gets interrupt signal then process will be stopped in running state and changed to ready state.


![[Pasted image 20230506201624.png]]


#### CPU and IO Bound processes:

* If the process is intensive in terms of CPU operations then it is called as CPU bound process.
* If the process is intensive in terms of IO operations then it is called IO bound process.

**Preemption:** Process is forcefully removed from CPU. pre-emotion is also called time sharing or multitasking.

**Non-preemption:** Processes are not removed until they complete the execution.