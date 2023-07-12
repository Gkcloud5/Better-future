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

### 1. What is subnetting?

* Network can be need to divide as per the organizations require.
* Organization subdivides the allocated address space into smaller allocations for each subnetwork within the organization, using a process called subnetting.
	* Result of subnetting is the number of subnetwork increases, while the number of usable host IP addresses decreases.
		* Each subnetwork is known as an IP subnet.


### 2. Why use subnetting?

* Subnetting enables assigned network addresses to be broken into smaller.
* Subnetting and route summarization work together to make routers more efficient by reducing the size of routing tables.

##### 2.1 Some steps:

* IP addresses must be unique on the internet when using public IP addresses.
* IPv4 addresses are 32bits made up of 4 octets of 8 bits each.
	* To calculate the subnet mask, convert an IP address to binary, perform the calculation and then convert back to the IPv4 decimal number.
* Subnet mask tells the computer what part of the IP address is the network portion of the address and what part identifies the host address range, which are addresses that are assigned to host computers on the network.
* Subnetting breaks a large network into smaller networks by extending the length of the subnet mask.
	* This increase the number of subnet mask
* Recent days classless IP address with VLSM are used almost exclusively to subnet a network.
* Default gateway is a device, typically router, where hosts sends packets that are destined for a device not on the local LAN.

### 3. Using the host's formula:

* it used to decide what subnet mask need to to in network
* **2^h - 2
	* h --> the number of 0s in subnet mask

##### 3.1 Find host range:
* Let consider we have 20 hosts in network, simplest thing to do would be to use `255.255.255.0` as your subnet mask.
	* This would mean you would have `192.168.0.1` through `192.168.0.254` for your hosts.
	* Address space reserved for subnet identifier `192.168.0.0`
	* Broadcast address `192.168.0.255`

##### 3.2 Convert to binary:
* 