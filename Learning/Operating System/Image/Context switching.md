#### Source:
[GFG](https://www.geeksforgeeks.org/measure-time-spent-context-switch/)
[YT](https://www.youtube.com/watch?v=W8vM3Qn-1aM&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=11)

* It's basically switching a CPU from one process to another process, while switching it saves a state of process so that the process will be resumed from their last state.
* It is the process of storing and restoring the state of a process or thread so that execution can be resumed from the same point at a later time.
* the CPU can only execute one process at a time, so the OS has to switch between processes to give the illusion of concurrent execution.