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
* 