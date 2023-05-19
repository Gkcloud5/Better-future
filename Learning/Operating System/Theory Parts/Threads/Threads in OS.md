#### Source:
[GFG](https://www.geeksforgeeks.org/thread-in-operating-system/)
[YT](https://www.youtube.com/watch?v=x1tg2YUCs-c&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=15)


#### What is thread?

* Thread means light weight process, it only contains limited number of instruction.
* Thread address space is associated with process address space
* within a program, a thread is a separate execution path.
* The OS creates and manages threads and they share the same memory and resources as the program that created them. this enables threads to collaborate and work efficiently within a single program.
* Threads share the same address space, code and data segments, but they have their own stack and program counter.

#### Why do we need thread?

* Threads run in parallel improving the application performance. Each such thread has its own CPU stage and stack, but they are share the address space of the process and the environment.
* Threads can share common data so they do not need to use Interprocess communication. Like the processes, threads also have states like ready, executing, blocked
* Priority can be assigned to the threads like process.
* [[TCB]]
* 