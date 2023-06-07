---
creation date: 2023-06-07 15:15
modification date: Wednesday 7th June 2023 15:15:45
tag: 
---

#### Source:
[LJ](https://linuxjourney.com/lesson/tcp-ip-model)

--------------------------------------

#### Explanation about it:

* TCP/IP model is actually what the internet is based off of.
* It is the actual implementation of networking
* It uses TCP/IP protocol suite, this protocol work together to specify how data should be gathered, addressed, transmitted and routed through a network.

##### Application layer:

* This is a top layer of TCP/IP. it determines how your computer programs interface with the transport layer services to view the data that gets sent or received.
* This layer uses
	* HTTP
	* SMTP

##### Transport layer:

* How data will be transmitted, includes checking the correct ports, the integrity of the data and basically delivering our packets.
* This layer uses
	* TCP
	* UDP

##### Network layer:

* This layer specifies how to move packets between hosts and across networks.
* This layer uses:
	* IP       - Helps route packets from one machine to another
	* ICMP - Helps tell us what is going on, such as error messages and debugging information.

##### Link layer:

* Link layer specifies how to send data across a physical piece of hardware. such as data travelling through ethernet, fiber