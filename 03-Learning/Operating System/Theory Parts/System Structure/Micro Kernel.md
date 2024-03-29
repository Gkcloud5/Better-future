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

![[Pasted image 20230429165340.png]]

* Micro kernel includes basic needs like process scheduling mechanism, memory and Interprocess communication.
* Micro kernel is a responsible for the OS most significant services, which are as follow
	* Inter-process communication
		* It refers to how processes interact with one another.
		* A process has several threads. in the kernel space, threads of any projects interact with one another.
		* Messages are sent and received across threads using ports.
	* Memory Management
		* It is process of allocating a space in memory for process.
		* Micro kernel create virtual memory if it's need
	* CPU scheduling
		* It is refers to which process the CPU will execute next.
		* It is helped to optimize a CPU utilization.
		* minimize a waiting time for process
