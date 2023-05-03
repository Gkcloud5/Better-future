#### Source:
[ML vs MK](https://www.geeksforgeeks.org/monolithic-kernel-and-key-differences-from-microkernel/)

#### About monolithic:

* It is same like microkernel but here user services and kernel services are implemented under the same address space.
* It increases the size of the kernel, thus increasing the size of the OS as well.
* Kernel provides CPU scheduling, memory management, file management and other system functions through system calls.
	* both services are implemented under the same address space, this makes OS execution faster.
* 