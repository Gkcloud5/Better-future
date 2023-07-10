---
creation date: 2023-07-09 15:51
modification date: Sunday 9th July 2023 15:51:50
---

**Tags:** 

#### Source:
[tt](https://www.techtarget.com/searchnetworking/definition/variable-length-subnet-mask#:~:text=Variable%20Length%20Subnet%20Mask%20(VLSM)%20is%20a%20subnet%20%2D%2D%20a,A%2C%20B%20or%20C%20network.)
[CG](https://chat.openai.com/share/b677b8c4-b342-444c-902b-83b53c528070)

--------------------------------------

#### Explanation about it:

* Variable length subnet mask
* It is a technique used in computer networking to allocate IP addresses to subnets with different sizes.
* VLSM allows network administrators to divide an IP address space into subnets of various sizes.
	* Which can help optimize the use of IP addresses and improve network efficiency.

#### VLSM fundamentals:

##### Subnet mask:
* Every device on a network has an IP address.
* A subnet mask splits this IP address into the host and network addresses.
	* This helps define which part of the IP address belongs to the network and which part belongs to the device
* A subnet mask is a 32-bit number, where all the host bits are set to 0
	* And the network bits are set to 1.
	* So the subnet mask consist of a sequence of 1s followed by a block of 0s.
		* Where the 1s represent the network prefix and the 0s mark the host identifier.

##### Subnetting:
* In subnetting, a large network is logically or physically divided into multiple small networks or subnets. the reason for subnetting a large network is to address network congestion and its negative impact on speed and productivity.
* Subne