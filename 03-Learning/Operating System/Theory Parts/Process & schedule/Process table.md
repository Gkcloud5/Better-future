#### Source:

[GFG](https://www.geeksforgeeks.org/process-table-and-process-control-block-pcb/)
[JTP](https://www.javatpoint.com/os-attributes-of-a-process)
[YT](https://www.youtube.com/watch?v=clYXGBVuEgE&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=8)


#### Process control block:

* Every process represented in OS with help of PCB.
* It specify information about process.
* PCB gives identity to each process so that OS can easily distinguish between process.

![[Pasted image 20230507141132.png]]

##### Pointer:

* It is a stack pointer which is required to be saved when the process is switched from one state to another to retain the current position of the process.
	* Stack pointer is a small register that stores the memory address of the last data element added to the stack.
##### Process state:

* It represents process state
	* ready, wait, running, ...

##### Process number:

* Each process will have unique ID that id called as process number.
* Process ID.

##### Program counter:

* It always contain a address of next instruction to be executed.

##### CPU registers:

* It used to store data.
* Every process has its own set of registers which are used to hold the data which is generated during the execution of the process.

##### CPU scheduling information:

* It have information regarding scheduling like round robin, priority.

##### Memory Management information:

* This contains information about memory management system used by OS. this may include the page tables, segment tables.

##### Accounting information:

* It means store information about CPU, how much time CPU executing a process

##### List of open files:

* It maintain files which are opened for this process.

##### List of IO devices:

* What are the IO devices are allocated for process.