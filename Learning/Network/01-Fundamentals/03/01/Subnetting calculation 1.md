---
creation date: 2023-07-12 14:43
modification date: Wednesday 12th July 2023 14:43:45
---

**Tags:** #network 

#### Source:
[TT](https://www.techtarget.com/searchnetworking/tip/IP-addressing-and-subnetting-Calculate-a-subnet-mask-using-the-hosts-formula)

--------------------------------------

#### Explanation about it:

### [[How to calculate subnet mask]]

### What is subnetting?

* Network can be need to divide as per the organizations require.
* Organization subdivides the allocated address space into smaller allocations for each subnetwork within the organization, using a process called subnetting.
	* Result of subnetting is the number of subnetwork increases, while the number of usable host IP addresses decreases.
		* Each subnetwork is known as an IP subnet.


### Why use subnetting?

* Subnetting enables assigned network addresses to be broken into smaller.
* Subnetting and route summarization work together to make routers more efficient by reducing the size of routing tables.

##### Some steps:

* IP addresses must be unique on the internet when using public IP addresses.
* IPv4 addresses are 32bits made up of 4 octets of 8 bits each.
	* To calculate the subnet mask, convert an IP address to binary, perform the calculation and then convert back to the IPv4 decimal number.
* Subnet mask tells the computer what part of the IP address is the network portion 