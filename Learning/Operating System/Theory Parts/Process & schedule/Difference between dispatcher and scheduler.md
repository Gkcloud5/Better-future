#### Source:
[GFG](https://www.geeksforgeeks.org/difference-between-dispatcher-and-scheduler/)

#### Scheduler:

* Scheduler responsible for deciding which process should be executed next. It determines which process is most deserving of the CPU time based on the scheduling algorithm used, such as round-robin, priority based or shortest job first.


#### Dispatcher:

* Once the scheduler selects the next process to execute, the dispatcher is responsible for loading that process into memory and giving it control of the CPU. 
* It performs context switching, saving the state of the previously running process and restoring the state of the new process.
* The dispatcher is responsible for transferring control of the CPU from one process to another