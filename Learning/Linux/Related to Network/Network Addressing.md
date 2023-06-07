---
creation date: 2023-06-07 22:06
modification date: Wednesday 7th June 2023 22:06:54
tag: #kernel #Linux #OS
---

#### Source:
[LJ](https://linuxjourney.com/lesson/network-addressing)

--------------------------------------

#### Explanation about it:

* Packets need the sender and receiver information.
	* This info can be gathered by MAC addresses and IP addresses.

##### MAC addresses:

* MAC address is a unique identifier used as a hardware address.
* This address will never change.
* When you want to get access to the internet, your machine needs to have network interface card.
* This network adapter has its own address
	* That's used to identify your machine.
* MAC addresses are given to network adapters when they are manufactured.

##### IP addresses:

* IP address is used to identify a device on a network.
* it is hardware independent and can vary in syntax depending on if you are using ipv4 or ipv6.

**Packets takes both software and hardware to move across network, so we have 2 identifiers MAC(hardware), IP(software)**


##### Hostnames:

* One last way to identify your machine is through hostname.
* Hostname take your IP address and allow you to tie that address to human readable name
* like myhost.com