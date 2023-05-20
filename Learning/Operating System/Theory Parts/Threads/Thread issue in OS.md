#### Source:
[YT](https://www.youtube.com/watch?v=dHB1UNv5I10&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=18)


* While implementing multi-threading we need to consider several thread


#### Fork system call and exec system call:

* Generally, fork system call will help to create new process it's exact duplicate of a parent process,
* exec system call used to inorder replace duplicate process with new process.
* Let consider fork system call in thread 1 so new process is created with 1 thread or same thread count as parent thread.
* Two options:
	* exec() system call after executing fork system call so exec process will replace a newly created process by fork
	* No exec system call 