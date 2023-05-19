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
* Threads can also help to improve the **scalability** of applications by allowing them to handle more requests them to handle more requests at the same time.
* **Improved performance:** threads can improve performance by allowing multiple tasks to be executed concurrently.
* **Reduced development time:** Threads can help to reduce development time by allowing developers to focus on logic of their application rather than on the details of how to manage multiple tasks.

#### Difference between process and thread:

![[Pasted image 20230519185601.png]]

**Main difference between process and thread is that a process is a complete program in execution, whereas a thread is lightweight sub-unit of process that can run concurrently with other threads in the same process.**

![[Pasted image 20230519185853.png]]


#### [[Single thread]]

