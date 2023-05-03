#### Source:
[ML vs MK](https://www.geeksforgeeks.org/monolithic-kernel-and-key-differences-from-microkernel/)

#### About monolithic:

* It is same like microkernel but here user services and kernel services are implemented under the same address space.
* It increases the size of the kernel, thus increasing the size of the OS as well.
* Kernel provides CPU scheduling, memory management, file management and other system functions through system calls.
	* both services are implemented under the same address space, this makes OS execution faster.

![[Pasted image 20230504030041.png]]

**If any service fails then the entire system crashes**


#### Key diff between monolithic and micro kernel:

* **System services**:
	* In monolithic, all the system services run in kernel space
	* In microkernel, only the most basic services(memory and process schedule) run in kernel space, with other services running in user space
* **Performance:**
	* Monolithic kernel are generally faster and more efficient than microkernels
		* Because there is no need to move a data between kernel space to user space
* **Modularity:**
	* Microkernel are more modular than monolithic kernels
		* Because, add or remove a services are very easy in microkernel
* **Security:**
	* Microkernels are generally considered more secure than monolithic kernel.
		* Because a bug or vulnerability in a service running in user space is less likely to affect the entire system.

![[Pasted image 20230504031157.png]]


![[Pasted image 20230504031244.png]]


![[Pasted image 20230504031324.png]]

