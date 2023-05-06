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
	* Reason for this is we don't know how much they 