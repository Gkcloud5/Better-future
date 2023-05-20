#### Source:
[GFG](https://www.geeksforgeeks.org/benefits-of-multithreading-in-operating-system/)

### Benefits:

#### Responsiveness:

* Multithreading in an interactive application may allow a program to continue running even if a part of it is blocked or performing a lengthy operations. it will increase a responsiveness to the user.
* If a non-multi threaded environment, a server listens to the port for some request and when the request comes, it processes the request and then resume listening to another request. the time taken while processing of request makes other users wait unnecessarily.

#### Resource sharing:

* Process may share resource by following techniques
	* Message passing
	* Shared Memory
* Such techniques must be explicitly organized by programmer.
* Threads share the memory and the resources of the process to which they belong by default.


#### Economy:

* Allocating memory and resources for process creation is a costly job in terms of time and space.
* Since, threads share memory with the process it belongs, it is more economical to create