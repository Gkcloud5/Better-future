#### Source:
[GFG](https://www.geeksforgeeks.org/kernel-i-o-subsystem-in-operating-system/)


* Kernel provides many services related to IO.
* Several services such as
	* Scheduling
	* Caching
	* Spooling
	* error handling
* IO subsystem is also responsible for protecting itself from errant processes and malicious users.


#### IO scheduling:

* To schedule a set of IO requests, to determine a good order in which to execute them
* The order in which the application issues the system call.
* Scheduling can improve the overall performance of the system.
* It reduce the average waiting time, response time and turnaround time for IO.


#### Buffering:

* A buffer is a memory area that stores data being transferred between two devices or between a device and an application.