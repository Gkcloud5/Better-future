#### Source:

[GFG](https://www.geeksforgeeks.org/process-table-and-process-control-block-pcb/)
[JTP](https://www.javatpoint.com/os-attributes-of-a-process)
[YT](https://www.youtube.com/watch?v=clYXGBVuEgE&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=8)


#### Process control block:

* Every process represented in OS with help of PCB.
* It specify information about process.
* PCB gives identity to each process so that OS can easily distinguish between process.

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

##### CPU scheduling information:

* It have information regarding scheduling like round robin, priority.

##### Memory Management information:

* This contains information about memory management system used by OS. this may include the page tables, segment tables.

##### Accounting information:

* It means store information about CPU, how much time CPU executing a process

##### 