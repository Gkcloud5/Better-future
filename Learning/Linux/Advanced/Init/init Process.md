---
creation date: 2023-06-04 22:57
modification date: Monday 5th June 2023 20:08:45
tag: #linux #OS #init #kernel
---

#### Source:
[LJ](https://linuxjourney.com/lesson/sysv-overview)

-----------------------------------------------------
#### What is it?

* Main purpose of init process is to start and stop essential processes on the system.
* it has a process id of 1 and serves as the ancestor of all other processes in the system.
* init process is a responsible for initializing the system and starting essential services and daemons.[[Daemons in Linux]]
-----------------------------------------------------
#### Why we need it?

* It is also known as father of all the process.
* It ensures that all of the necessary processes are started when the system boots up.
* It helps to keep the system stable, if a process crashes, the init process can restart it.

-----------------------------------------------------
#### Where it comes?

* It comes under a kernel booting process.
* Init is a first process executing in OS.
-----------------------------------------------------
#### Explanation about it:

* Different versions of linux have used different init systems. the most common init systems are:
	* [[System V]]
	* [[Upstart]]
	* [[Systemd]]
* 
-----------------------------------------------------
#### Benefit:


-----------------------------------------------------
#### Simple Explanation:


-----------------------------------------------------
#### Visual image of topic:


-----------------------------------------------------

#### Links: