---
creation date: 2023-06-10 15:14
modification date: Saturday 10th June 2023 15:14:32
tag: 
---

#### Source:
[LJ](https://linuxjourney.com/lesson/distance-vector-protocols)

--------------------------------------

#### Explanation about it:

* Distance vector protocol determine the path of other networks using the hop count a packet takes across the network.
* It is a routing protocol used in computer networks to determine the best path for data packets to travel from source to destination.
* If a network A was 3 hops away and network B was next to network A, then we assume it must be 4 hops away, in distance vector protocol, the next route would be one with the lease amount of hops.
* One of the most common distance vector protocol is RDP(Routing information protocol), it broadcasts the routing table to every router in the network every 30 seconds.