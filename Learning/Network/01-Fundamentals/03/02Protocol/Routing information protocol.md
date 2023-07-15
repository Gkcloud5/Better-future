---
creation date: 2023-07-15 13:21
modification date: Saturday 15th July 2023 13:21:02
---

**Tags:** #network #protocol 

#### Source:
[RIP](https://www.scaler.com/topics/routing-information-protocol-rip/)

--------------------------------------

#### Explanation about it:

* RIP is a distance vector routing protocol.
* Routers that use the distance vector protocol send all or portion of their routing tables to their neighbors in routing update messages.
* RIP employs a distance vector algorithm to determine which path a packet should take to reach its destination.
* Each RIP router maintains its routing table, which lists all the destinations the router knows how to reach.
* In every 30 seconds, each router broadcasts its whole routing table to its closest neighbors.

### Introduction:

* RIP is a dynamic routing protocol that finds the optimum path between the source and destination networks by using hop count as a routing metric.

![[Pasted image 20230715132821.png]]


### Working of RIP:

* The RIP protocol is based on the [[Distance Vector Algorithm|distance vector algorithm]], one of the widely used routing algorithms that routers employ to dynamically determine the cost or metric of each potential path via the internetwork.
* Each RIP router maintains its routing table, which lists all the destinations the router knows how to reach.
	* In every 30 seconds, each router broadcasts its whole routing table to its closest neighbors.
* A router will update its table entry with the length and next hop address of the shortest path if it receives an update on a route and the new path is shorter.