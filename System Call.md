#### Source:
[SC-GFG](https://www.geeksforgeeks.org/introduction-of-system-call/)
[YT-1](https://www.youtube.com/watch?v=d3aCjfuMCIU&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=5)

#### About System Call:

* System Call is a interface between process and OS
	* Process means programs during the execution

#### Types of System Calls:

* **Process Control:**
	* Create a process
	* Terminate a process
	* Load a process
	* Execute a process
	* Wait
	* signal -- acknowledgement
	* Allocate and free a memory
* **File Management**
	* Create a file
	* Open a file
	* Read and copy
	* close a file
	* delete a file
* **Device Management**
	* Input or output devices
	* request a device
	* release a device
* **Information Maintenance**
	* It is mainly used to get the information about computer, information about process and information about file
	* Get time or date
	* set time or date
	* get process info
* **Communication**
	* One process can communicate with another process with a help of IPC
	* Creating a communication link
	* send and receive data
	* Delete communication link


#### Feature of System Calls:

* **Interface**
	* System calls provide interface between user program and the OS.
	* Program make requests by running specific functions, and the OS responds by executing the requested service and returning a result.
* **Protection**
	* System calls are used to access privileged operations that are not available to normal user programs. 
	* OS uses this privilege to protect the system from malicious or unauthorized access.
* **Kernel Mode**
	* When a system call is made, the program is temporarily switched from user mode to kernel mode.
	* In kernel mode, the program has access to all system resources, including hardware, memory and other processes.
* **Context switching**
	* System call requires a context switch, which involves saving the state of the current process and switching to the kernel mode to execute the requested service.
	* This can introduce overhead, which can impact system performance.
* **Error Handling**
	* System call can return error codes to indicate problems with the requested service. 
	* Program must check for these errors and handle them appropriately.
* **Synchronization**
	* System calls can be used to synchronize access to shared resources.
		* Such as file or network connections.