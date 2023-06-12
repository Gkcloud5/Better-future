---
creation date: 2023-06-12 10:32
modification date: Monday 12th June 2023 10:32:37
tag: 
---

#### Source:
[LJ](https://linuxjourney.com/lesson/link-state-protocols)

--------------------------------------

#### Explanation about it:

* Link state protocol are great for large scale networks, they are more complex than distance vector protocols.
* Here instead of sending out the whole routing table, they only send updates to neighboring routes.
* Link state protocol, each router collects information about its directly connected links, such as their state, bandwidth and delay. this information is then packaged into a message called a Link state ad and distributed to all routers in the network.
* Upon receiving LSAs from other routers, each routers constructs a map of the entire network called a link state database. the LSDB contains information about all the routers, links and their associated characteristics.
* Using the LSDB. each router independently calculates the shortest path to every destination in the network using a shortest path algorithm
* One of the common link state protocol is OSPF(Open shortest path finder), it only update the routing tables id there was a network change.