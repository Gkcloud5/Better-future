---
creation date: 2023-07-14 16:28
modification date: Friday 14th July 2023 16:28:09
---

**Tags:** #network #ospf

#### Source:
[OSPF](https://www.cloudflare.com/learning/network-layer/what-is-routing/)
[GG](https://www.geeksforgeeks.org/open-shortest-path-first-ospf-protocol-states/)
[SR](https://www.scaler.com/topics/ospf-protocol/)

--------------------------------------

#### Explanation about it:

* OSPF protocol is one of family of IP routing protocols.
* It is used to find the best path between source and the destination router using its own shortest path first.
* The protocol which aims at moving the packet within a large autonomous system or routing domain.
* It is a network layer protocols.
* OSPF is one of the intradomain protocols.
	* Intradomain protocol means that his protocol is used within the network or an area.
* OSPF protocol is the protocol that works based on the [[link State routing algorithm]] in which each router has the information about each domain and uses this information to determine the shortest path.

![[Pasted image 20230714192516.png]]

### Working of OSPF:

* First step in the working of OSPF protocol is to become the OSPF neighbors.
	* Two routers that are running on the same link and are connected establishes the neighbors relationship between them.
* Next step is to exchange the database information between the routers.
	* When the router establishes the neighbor relationship they exchange the link state database with each other.
* Third step in the working of the OSPF protocol is to select the best route.
	* After an exchange of LSDB information, the router find the best route for adding to the routing table.