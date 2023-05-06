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

#### 3. Running:

* It means CPU executing a process, if one process is executing in CPU then that process status will be running state.

#### 4. Waiting:

* A process while in running state, if it need some IO operation then process will move to waiting state.
* Once IO completed process will move to ready state.

#### 5. Terminated:

* If process completed all the operation then it will moved to

### Operations on the process:

#### 1. Scheduler:

* It allocate process from ready to CPU that means change process state to running.

#### 2. Interrupt:

* whenever process gets interrupt signal then process will be stopped in running state and changed to ready state.
