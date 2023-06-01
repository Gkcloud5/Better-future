**Process** --> **Threads**

#### Source:
[YT](https://www.youtube.com/watch?v=ZXW-iVivWF4&list=PL3uLubnzL2Tlbyrr2GFVRE7Azo8FJe-dJ&index=12)


#### What is a thread:

* Thread is not a process
* It is smaller unit.
* A process can create multiple thread
* Threads are not easy to track
* Each thread have unique id
	* We can identify it by using thread
* thread represents an independent sequence of instructions that can be scheduled and executed concurrently with other threads within the same process.
* Threads share the same memory space and resources of their process.
* [[Threads]]


##### Thread creation:

* Threads are typically created within a process by the OS or by the program itself using thread creation functions or system calls.
* Each thread has its own program counter, stack and set of registers.

##### Lightweight:

* It consumes fewer system resources compared to processes.
* creating and switching between threads is generally faster and requires less overhead than creating and switching between process.

##### Concurrency:

* Threads within a process can execute concurrently, meaning they can be scheduled to run simultaneously on different processors or CPU cores.
* This allows for parallel execution and can lead to improved performance and responsiveness in multi-threaded applications.