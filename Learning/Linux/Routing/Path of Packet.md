---
creation date: 2023-06-09 14:35
modification date: Friday 9th June 2023 14:35:10
tag: 
---

#### Source:
[LJ](https://linuxjourney.com/lesson/path-of-a-packet)

--------------------------------------

#### Explanation about it:

##### Packets travels within its local network:

* First the local machine will compare the destination IP address to see if it's in the same subnet by looking at its subnet mask.
* When packets are sent they need to have a source MAC address, destination MAC address, source IP address and destination IP address, at this point we do not know the destination MAC address.
* To get to the destination host, we use ARP to broadcast a request on the local network to find the MAC address of the destination host.
* Now the packet can be successfully sent.

##### How packets travels outside its network:

* First the local machine will compare the destination IP address, since its outside of our network, it does not see the MAC address of the destination host. And we can't use ARP because the ARP request is a broadcast to locally connected hosts.
* So our packet now looks at the routing table, 