#### Source:
[DM](https://www.geeksforgeeks.org/dual-mode-operations-os/)


* An error in one program can adversely affect many processes, it might modify data of another program or also can affect the OS.
* To ensure the proper execution of the OS, there are two modes of operation
	* User mode
	* Kernel mode

#### User mode:

* When the computer system is run by application like creating a text document or using any application program, then the system is in user mode.
* When the user application requests for a service from the OS then there will be a transition from user to kernel mode to fulfil request.

![[Pasted image 20230505155647.png]]



#### Kernel Mode:

* When the system boots, the hardware starts in kernel mode and when the OS is loaded, it starts user application in user mode.
* To provide protection to the hardware, we have privileged instructions which execute only in kernel mode.
