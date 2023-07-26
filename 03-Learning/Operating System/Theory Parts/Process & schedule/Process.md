#### Source:
[Process](https://www.geeksforgeeks.org/introduction-of-process-management/)
[YT-1](https://www.youtube.com/watch?v=udOPPbQhASg&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=6)

#### What is a process:

* A process means a program in execution
	* Program means collection on instruction inorder to perform specific task.
* At the time of execution OS moves program from hard disk to main memory then CPU can execute that program.
	* CPU can access only main memory.


#### What does a process look like in main memory?

![[Pasted image 20230506111801.png]]

**Text**   - Code segment, it stores instruction of a program.
**Data**  - It mainly stores global variable or static variable
**Heap** - To store dynamic memory allocation variable(pointer)
*Dynamic memory allocation means allocating memory during program run time*
**Stack** - It called as function stack.  if function have any arguments then those arguments store here

* Heap always grow upside, Stack always grow downside
	* why because we don't know which segment use more memory.


#### Some system call related to process:

1. Create a child process identical to the parent
2. Terminate a process
3. Wait for child process to terminate
4. Change the priority of process
5. Block the process
6. Ready the process
7. Dispatch a process
8. Suspend a process
9. Resume a process
10. Delay a process
11. Fork a process

#### Attributes or characteristics of a process:

1. **Process Id:** A unique identifier assigned by the OS
2. **Process State:** Can be ready, running, etc
3. **CPU registers:** Like the program counter
	1. CPU registers must be saved and restored when a process is swapped in and out of CPU.
4. **Accounts information:** Amount of CPU used for process execution, time limits, execution ID etc
5. **I/O status information:** For example, device allocated to the process, open files, etc
6. **CPU Scheduling information:** like priority(SJFS)