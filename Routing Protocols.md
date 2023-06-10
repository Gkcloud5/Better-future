---
creation date: 2023-06-10 14:28
modification date: Saturday 10th June 2023 14:28:18
tag: 
---

#### Source:
[LJ](https://linuxjourney.com/lesson/routing-protocols)

--------------------------------------

#### Explanation about it:

* Routing protocol are used to help  our system adapt to network changes.
* It learns of different routes, builds them in the routing table and then routes our packets through that way.
* Two primary routing protocol types
	* Distance Vector protocol
	* Link state protocol

##### Convergence:

*  It refers to the process by which routers within a network reach a consistent and synchronized understanding of the network's topology and the best paths for forwarding data.
* It involves the exchange of routing information, updating routing tables, and establishing stable routing paths after a change or disruption in the network.
* When using routing protocols, routers communicate with other routers to collect and exchange information about the network.
	* When they agree on how a network should look, every routing table maps out the complete topology of the network, thus converging.
	* when something occurs in the network topology, the convergence will temporarily break until all routers are aware of this change.