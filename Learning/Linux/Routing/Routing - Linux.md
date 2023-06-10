---
creation date: 2023-06-08 20:19
modification date: Thursday 8th June 2023 20:19:28
tag: 
---

#### Source:
[LJ](https://linuxjourney.com/lesson/what-is-a-router)

--------------------------------------

#### Explanation about it:

##### What is a router:

* Router enables machines on a network to communicate with each other as well as the other networks.
* On a router, we have LAN ports, that allow your machines to connect to the same LAN and you will also have an internet uplink port that connects you to the internet.
* Router decides where our network packet go and which ones come in.
* It routes our packet multiple networks to get from it's source host to it's destination host.


##### How does router work?

* Router is a networking device that operates at the network layer(layer3) of the OSI model.
* Its primary function is to forward data packets between different networks, allowing devices to communicate with each other.
* Router receives data from your devices. this data can be anything from a webpage request to an email.
* Router converts the data into a format that can be transmitted over the internet. this is done by breaking the data down into small pieces called packets.
* The router sends the packets out to the internet. the packets are sent to the router that is closest to the destination server.
* the packets are routed through the internet until they reach the destination server.
* the destination server reassembles the packets and sends the data back to the router.
* router converts the data back into its original format and sends it to your device.


##### Additional details about router:

* Router has two interfaces
	* WAN interface -  it used to connect to internet
	* LAN interface - it used to connects home network
* Routers using routing protocol to determine the best path to send data.
	* The most common routing protocol is called RIP(Routing information protocol)


[[Routing Table - Linux]]

[[Path of Packet]]

[[Routing Protocols]]

[[Distance vector protocol]]



