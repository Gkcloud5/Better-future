#### Source:
[YT](https://www.youtube.com/watch?v=fSMVWmGPqlM&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=13)

#### What is Interprocess communication:
* Interprocess communication refers to the mechanisms and techniques used by processes running on the same computer or across network to exchange data, share resources and coordinate their activities.
* It allows processes to communicate with each other.
* IPC means how one process communicate with other process
* In multiprogramming system multiple process resides in main memory, so one process can communicate with another process with a help of IPC.

#### Advantage of IPC:

##### Information Sharing:
* Each process can share some message with other process.
	* IO device
	* Printer
	* Scanner

##### Modularity:
* If there is big module(task) then it divided into small tasks, so the small task perform their own tasks.

##### Computational Speedup:
* Big task divided into small task and all small task perform concurrently so time will be saved.

##### Convenience:
* It is very convenient for users because it will help us to do multiple task efficient manner

#### Mechanism:

**In order to implement IPC they have two mechanism, that's are**
* Shared Memory
* Message Passing

##### Shared Memory:

 ![[Pasted image 20230513225623.png]]

* We have 2 process p1 and p2 and have shared memory.
* It is very very faster because it don't need any system call.
* Here p1 can communicate with p2 with a help of shared memory.

##### Example for shared memory:
* Let assume producer and consumer problem,

![[Pasted image 20230514141954.png]]

