---
creation date: 2023-06-14 21:29
modification date: Wednesday 14th June 2023 21:29:39
tag: 
---

#### Source:
[LJ](https://linuxjourney.com/lesson/icmp)

--------------------------------------

#### Explanation about it:

* ICMP stands for internet control message protocol, it is a network protocol that is used to send error messages and control messages and operational information between network devices.
* ICMP operates at the network layer of the TCP/IP protocol suite, and its primary purposes is to provide feedback and reporting about the status of network.
* It used to send updates and error messages and is an extremely useful protocol used for debugging network issues such as a failed packet delivery.
* Each ICMP message contains a type, code and checksum field.
	* type field is the type of ICMP message,
	* the code is a sub-type and describes more information about the message and the checksum is used to detect any issues with the integrity of the message.
* Common ICMP types
	* TYPE 0 - Echo reply
	* TYPE 3 - Destination unreachable
	* TYPE 8 - Echo request
	* TYPE 11 - Time exceeded