---
creation date: 2023-06-04 18:50
modification date: Sunday 4th June 2023 18:50:35
tag: #kernel
---

#### Source:
[LJ](https://linuxjourney.com/lesson/system-calls)

-----------------------------------------------------
#### What is it?

* System call provide user space processes a way to request the kernel to do something for us.
* The kernel makes certain services available through the system call API.
	* These services allow us to read or write to a file, modify memory usage, modify our network, etc.
* OS already has table of what system call exist and each system call has a unique ID.
* It is a programmatic method in which computer program requests a service from the kernel of the OS.
* It provide a way for user-level program to interact with the OS kernel.

![[Pasted image 20230604210613.png]]

----------------------------------------------------------------------

#### Why we need it?

* ##### Access to privileged instructions:
	* System call allow user-level programs to execute privileged instructions that are restricted from direct execution. this instructions might involve accessing hardware devices.
* ##### Resource Management:
	* System call enable programs to request and release system resources such as files, network connections and hardware devices.
* ##### Process control:
	* It allow programs to create, terminate and manage processes.

-----------------------------------------------------
#### Where it comes?

* System call is a bridge between user interface and kernel.

-----------------------------------------------------
#### Explanation about it:

* A system call is a way for a program running on a computer to request services from the OS.
* It acts as a bridge between user-level programs(application) and the low-level operations performed by the OS.
* Program passes specific parameters to the system call, indicating what it wants the OS to do.
* OS receives the system call, checks the validity of the request and performs the requested operation on behalf of the program.
* Once the OS completes the requested operation, it return control back to the program.

-----------------------------------------------------
#### Benefit:

* It helps OS to efficiently manage system resources.
* It play crucial role in enforcing security and protection mechanism.
* It will create, terminating and managing process.
* It can be used to Interprocess communication, like exchange data, share resources.
* It provide standardized interface for program to interact with the OS.

-----------------------------------------------------
#### Simple Explanation:

* System call helps user's program to access computer hardware with a help of kernel.
* It validity request from users so it consider security check also.
* By requesting and releasing resource, it will helps OS to utilize a resource more efficiently.
* it helps to manage process also

-----------------------------------------------------
#### Visual image of topic:

![[Pasted image 20230604212927.png]]

--------------------------------------------
#### Links:

[[System Call]]
