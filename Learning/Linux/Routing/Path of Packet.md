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
* So our packet now looks at the routing table, it does not know the address of the destination IP, so it sends it out to the default gateway(another router). 
	* So now our packet contains source IP, destination IP and source MAC, we don't have destination MAC addresses.
* The router looks at the packet and confirms the destination MAC address, but it's not the final destination IP address, so it keeps looking the routing table to forward packet to another IP address 
	* That can help the packet move along to its destination.
	* Everytime packet moves, it strips the old source and destination MAC address and updates the packet with the new source and destination MAC addresses.
* Once the packet gets forwarded to the same network, we use ARP to find the final destination MAC address.
* During this process, our packet does not change the source or destination IP address.