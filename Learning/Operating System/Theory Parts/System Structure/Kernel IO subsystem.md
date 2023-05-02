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
* Buffering is done for three reasons:
	* First is to cope with a speed mismatch between producer and consumer of a data stream.
	* 2nd use of buffering is to provide adaptation for data that have different data transfer sizes.
	* 3rd use is to support copy semantics for the application IO.
		* **Copy semantics** means suppose that an application wants to write a data on a disk that is stored in its buffer. it calls the `write()` system's call.


#### Caching:

* Caching is a region of fast memory that holds a copy of a data.
* Access to the cached copy is much easier than the original file.
* Main diff between buffer and cache is that a buffer may hold only the existing copy of a data item.
	* While cache, it holds a copy on faster storage of an item that resides elsewhere.


#### Spooling and device reservation:

*  