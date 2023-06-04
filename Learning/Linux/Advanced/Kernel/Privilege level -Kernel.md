---
creation date: 2023-06-03 23:21
modification date: Sunday 4th June 2023 17:29:22
tag: 
---

#### Source:
[LJ](https://linuxjourney.com/lesson/kernel-privilege-levels)
[S1](https://www.baeldung.com/cs/os-rings)
[S2](https://www.futurelearn.com/info/courses/computer-systems/0/steps/53514)
[S3](https://www.geeksforgeeks.org/protection-ring/)

-----------------------------------------------------
#### What is it?

* OS provide different level to access resources.
* This are hierarchically arranged from most privileged to least privileged.
* OS manages system resources, such as processing time on the CPU and access to memory
	* Computers are often running multiple software processes at once, and these will require differing levels of access to resources and hardware.
	* Process are executed in layered "rings". where each ring has different access rights to resources.

![[Pasted image 20230604181108.png]]

* Processes are executed in this protection rings then process has little limitation as per the ring process in.

-----------------------------------------------------
#### Why we need it?

* Protection rings are one of the key solutions for sharing resources and hardware.
* It protects the system against crashes.
* It offer increased security.

-----------------------------------------------------
#### Where it comes?

* OS have two different abstraction layer
	* Kernel space
	* User space
* Both layer operates in two different mode.
	* Kernel space operated in kernel mode
	* User space operated in user mode
* This privilege ring comes under a process, based on process it will placed in layer

-----------------------------------------------------
#### Explanation about it:

* It mainly provide limit to process to access a resources.
* the limitation is based on where is that process in layer.
* Levels of ring protection
	* Ring 0
	* Ring 3
	* Ring 1 and Ring 2

* ##### Ring 0:
	* It is accessible to the kernel, which is a central part of most OS and can access everything.
	* Code running here is said to be running in kernel mode.
	* Process running in kernel mode affect all the entire system if anything fails here
* ##### Ring 3:
	* It is a least privilege ring
	* It is accessible to the user processes that are running in user mode.
	* This ring has no direct access to the CPU or memory.
* ##### Rings 1 and 2:
	* It has special privileges that ring 3 does not.
	* Ring 1 is used to interact with and control hardware connected to your computer
	* Ring 2 is used for instructions that need to interact with system storage, loading and saving files.

-----------------------------------------------------
#### Benefit:

* It provides better control over the access of system resources.
* It ensures that the users only have access to the resources they are authorized to access, thus improving computer security.

-----------------------------------------------------
#### Simple Explanation:

* Kernel is a important thing to connect hardware and getting work from hardware so if any mistake happen in hardware while doing process it will affect hole computer process so we need to avoid this thing so that we can use privilege ring to control the hardware resources with different layer. not all layer have direct connection to hardware so mostly unexcepted thing not going to happen
-----------------------------------------------------
#### Visual image of topic: