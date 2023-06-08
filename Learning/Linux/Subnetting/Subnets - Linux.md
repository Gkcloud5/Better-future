---
creation date: 2023-06-07 23:21
modification date: Wednesday 7th June 2023 23:21:42
tag: 
---

#### Source:
[LJ](https://linuxjourney.com/lesson/subnets)

--------------------------------------

#### Explanation about it:

* A subnet is a group of hosts with IP addresses that are similar in a certain way.

##### Subnet masks:

* It determine what part of your IP address is the network portion and what part is the host portion.

```
255.255.255.0
```

* 255 portion is actually our mask.
* Subnetting is used to segment networks and control the flow of traffic within that network.
	* So a host on one subnet can't interact with another host on a different subnet.


