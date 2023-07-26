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

* A spool is a buffer that holds the output of a device, such as printer that cannot accept interleaved data streams.  although printer can serve only one job at a time, several applications may wish to print their output concurrently.
	* Without having their output mixes together.
* The OS solves this problem by preventing all output from continuing to the printer.
* output of all applications is spooled in a separate disk file. when an application finishes printing then the spooling system queues the corresponding spool file for output to the printer.

#### Error handling:

* OS uses protected memory can guard for against many kinds of hardware and application errors.
* So that complete system failure is not the usual result of each minor mechanical glitch, devices and IO transfer


#### IO protection:

* Errors and the issue of protection are closely related.
* A user process may attempt to issue illegal IO instruction to disrupt the normal function of a system.
* We can use various mechanisms to ensure that such disruption cannot take place in the system.


### kernel IO subsystem:

* It is a one of the critical component of a OS
* It is a interface between OS and input and output devices.
* It major work is get a input and output instruction from OS (made by application) and assign to hardware.