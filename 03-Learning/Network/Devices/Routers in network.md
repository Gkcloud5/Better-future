---
creation date: 2023-07-13 19:00
modification date: Thursday 13th July 2023 19:00:36
---

**Tags:** #network #routers

#### Source:
[Router](https://www.cloudflare.com/learning/network-layer/what-is-routing/)

--------------------------------------

### What is routing?

* Network routing is the process of selecting a path across one or more networks.
* The internet routing decisions are made by specialized pieces of network hardware called routers.

### What is a router? [](https://www.cloudflare.com/learning/network-layer/what-is-a-router/)

* A router is a device that connects two or more packet-switched networks or subnetworks.
* It server two primary functions
	* Forwarding data packets to their intended IP address
	* Allow multiple devices to use the same internet connection.
* [[Network switch]] forwards data packets between groups of devices in the same network, where a router forwards data between different networks.

### How does a router work?

* Think of a router as an air traffic controller and data packets as aircraft headed to different airports(network).
	* Each plan has a unique destination and follows a unique route, each packet needs to be guided to its destination as efficiently as possible.
		* In the same way that an air traffic controller ensures that planes reach their destinations without getting lost or suffering a major disruption along the way, a router helps direct data packets to their destination IP address.
* Router uses **Internal routing table** a list of paths to various network destinations.
	* The router reads a packet's header to determine where it is going, then consults the routing table to figure out the most efficient path to that destination.

### How does routing work?

* Router refers to internal routing tables to make decisions about how to route packets along network paths.
* A routing table records the paths that packets should take to reach every destinations that the router is responsible for.
* Router working way:
	* When router receives a packet, it reads the headers and get info about destination, then it determines where to route the packet based on information in its routing table.
	* Some times packets routed several times by different routers.
* Routing table may be static or dynamic.
	* Dynamic routing table update automatically.

### [[Main Routing Protocols]]
