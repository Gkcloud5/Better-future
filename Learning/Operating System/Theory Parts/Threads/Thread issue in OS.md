#### Source:
[YT](https://www.youtube.com/watch?v=dHB1UNv5I10&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=18)


* While implementing multi-threading we need to consider several thread


#### Fork system call and exec system call:

* Generally, fork system call will help to create new process it's exact duplicate of a parent process,
* exec system call used to inorder replace duplicate process with new process.
* Let consider fork system call in thread 1 so new process is created with 1 thread or same thread count as parent thread.
* Two options:
	* exec() system call after executing fork system call so exec process will replace a newly created process by fork
	* No exec system call only fork call so may create as many threads

#### Thread Cancellation:

* Killing a thread and eliminating a thread.
* Two Approach:
	* **Asynchronous:** Killing a thread immediately even that thread having a work.
	* **Deferred:** Once all the operation of thread completed then it will cancel it themself.

#### Signal Handling:

* Signal is a special notification which is sent from 1 process to another process or kernel may send signal to the process.
* Let consider p1 sends signal to p2 here p2 have 4 thread, so process p2 thread confusion with which thread need to handle event.