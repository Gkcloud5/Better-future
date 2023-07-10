---
creation date: 2023-07-10 16:54
modification date: Monday 10th July 2023 16:54:04
---

**Tags:** #network 

#### Source:
[YT](https://www.youtube.com/watch?v=c6ENgy21hyI)
[CF](https://www.cloudflare.com/learning/network-layer/what-is-a-subnet/)

--------------------------------------

#### Explanation about it:

### 1. What is subnet?

* A subnet, or subnetwork, is a network inside a network.
* Subnets make networks more efficient.
* Through subnetting, network traffic can travel a shorter distance without passing through unnecessary [[Routers in network]] to reach its destination.

![[Pasted image 20230710171929.png]]

* When are more efficient when messages travel as directly as possible.
* When a network receives data packets from another network.
	* It will sort and route those packets by subnet so that the packets do no take an inefficient route to their destination.


### 2. Why is subnetting necessary?

* As the previous example illustrates, the way IP addresses are constructed makes it relatively simple for internet routers to find the right network to route data into.
* However, in a class A network, there could be millions of connected devices, and it could take some time for the data to find the right device.
	* This is why subnetting comes in handy: subnetting narrows down the IP address to usage within a range of devices.

### 3. What is a subnet mask?

* 