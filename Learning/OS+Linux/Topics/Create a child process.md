#### Source:
[YT](https://www.youtube.com/watch?v=7VOW4zkDZrQ&list=PL3uLubnzL2Tlbyrr2GFVRE7Azo8FJe-dJ&index=6)
[child](https://www.includehelp.com/operating-systems/child-process-in-operating-system.aspx)


#### What is a child process in OS?

* One process can create another process, this methodology involves in multitasking OS
	* Here, the process creates another process is called the parent process and created process is referred to as the child process.
* Child process is a subprocess of a main process

#### Approaches for creating a child process:

* Two Approaches
	* By using **fork** system call
	* By using **spawn** system call

##### Fork system call:

* Most of the features of the parent process come into its child process.
* For example,
	* File descriptors come into subprocess from its parent
* In the unix system, a child process is referred to as the copy of its parent, using the fork system call.
* After the child process has created, it can be laminated with a different program(using exec system call) as per the requirement.

##### By using the spawn:

* Spawn is a method by which we can load and execute a new child process. currently, the running process can wait for the subprocess bring to an end or it can continue on its job.
* Any process that is n