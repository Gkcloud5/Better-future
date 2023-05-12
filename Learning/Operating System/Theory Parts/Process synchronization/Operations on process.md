#### Source:
[YT](https://www.youtube.com/watch?v=TWXdAaRsrMs&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=12)

#### Two operation:

1. Process creation
2. Process Termination

#### Process creation:

* A parent process can create several child process.
* A child process can create their own child process

![[Pasted image 20230512190707.png]]

##### Resource sharing:
* Wherever parent process create a child process then the parent process can shares all of its resources with the children process. or parent process share some of his resources with children or it never share any resources with children.

##### Execution:
* Parent and child process may execute concurrently
* Parent process has to wait until the child process completed.

##### Address space for child process:
* Child process is duplicate of parent process. child process have same PCB data of parent process only difference is process id.
* Child process can replaced with new process

##### UNIX example:
**Fork System call:**
It will create a child process from parent process, it create exact duplicate of parent process.

**EXEC system call:**
It replace duplicated process with new process.

 
![[Pasted image 20230512212634.png]]



#### Process Termination:
**EXIT system call:**
Once the operation of process all completed then the process will be terminated by calling exit system call.

**KILL System call:**
Sometime parent process need resource that allocated to child process, in this situation OS use kill system call and kill all the child process and then allocate freed resources to parent process