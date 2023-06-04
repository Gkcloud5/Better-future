---
creation date: 2023-06-03 23:21
modification date: Sunday 4th June 2023 17:29:22
tag: 
---

#### Source:
[LJ](https://linuxjourney.com/lesson/kernel-privilege-levels)
[S1](https://www.baeldung.com/cs/os-rings)
[S2](https://www.futurelearn.com/info/courses/computer-systems/0/steps/53514)

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

* 
-----------------------------------------------------
#### Explanation about it:


-----------------------------------------------------
#### Benefit:


-----------------------------------------------------
#### Simple Explanation:


-----------------------------------------------------
#### Visual image of topic: