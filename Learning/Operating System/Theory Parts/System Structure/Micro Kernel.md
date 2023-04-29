#### Source:

[Micro kernel](https://www.geeksforgeeks.org/microkernel-in-operating-systems/)
[MK-1](https://www.javatpoint.com/microkernel-in-operating-system)


#### What is kernel?

* Kernel is intermediate between application and hardware
* software --> kernel -> hardware
* Kernel helps to use hardware more effectively

#### What is Micro kernel?

* It handle all the system resources. 
* In a microkernel user and kernel services are implemented in distinct address spaces.
	* User services are kept in user address space
	* Kernel services are kept in kernel address space
* Adding a new service is very simple.
* If any module fails then orders are unaffected
	* because each module are represented specify address
* It provides a minimal amount of process and memory management services.

#### Architecture of Micro Kernel:
