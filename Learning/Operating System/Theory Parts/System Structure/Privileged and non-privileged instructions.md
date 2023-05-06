#### Source:
[P&NP](https://www.geeksforgeeks.org/privileged-and-non-privileged-instructions-in-operating-system/)

#### About privileged:

* Privileged instructions are those that can only be executed by the OS kernel. Such as
	* Device drivers
* These instructions typically perform operations that require direct access to hardware or other privileged resources. such as
	* setting up memory mapping
	* accessing i/o devices

#### About non-privileged:

* It can be executed by any process, including user-level processes. 
* These instructions are typically used for performing computations, accessing user-level resources such as files and memory, and managing process control.
* Non-privileged instructions are executed in user mode, which provided limited access to system resources and ensures that process cannot interfere with one another.


#### Key difference privileged and non-privileged instructions:

* **Access to resources:**
	* Privileged instructions have direct access to system resources, while non-privileged instructions have limited access.