#### Source:
* [Types](https://www.geeksforgeeks.org/types-of-operating-systems/)
* [Youtube-1](https://www.youtube.com/watch?v=GWsxSvdd09o&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=3)

#### Types:

##### Batch system:
* Batch means collection of jobs
* User uses **Punch cards**, user provide job information in the form of punch cards.
* After writing instruction in punch cards, will submit to computer operator
	* Operator will batch the instruction as per their category and process it
* In this OS, users not possible to interact with computer directly.
* CPU idle time is high in this OS.

##### Multiprogrammed system:
* We place multiple program to main memory and execute all the program simultaneously.
* Main usage of this OS is we can use CPU effective manner.

##### Time Sharing System:(Multitasking System)
* It is a extension to a multiprogrammed system, here also multiple program is contain in main memory and executed simultaneously.
* CPU allocates time to all the process to execute.
* CPU idle time is very low here

##### Multiprocessor system:
* Here instead of single processor multiple processor connected to a same computer.
* Advantages:
	* It increase a **throughput**. in lessor span of time we will get output.
	* **Economy**: It is very cheap because we have a multiple processor in a single computer
	* **Reliability:** If one processor failed then another processor will execute a instruction.

##### Distributed System:
* Same information is distributed to all the corresponding systems in network, due to some problem if any system failed then all of other system will continue a work

##### Real Time OS:
* It used to build real time application.
* Two type:
	* Hard real time:
		* Application should be executed within time
	* Soft real time:
		* If any problem then it will does not affect a process, it will execute successfully.