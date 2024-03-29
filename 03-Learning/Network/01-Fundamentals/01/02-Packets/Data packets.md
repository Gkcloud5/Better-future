---
creation date: 2023-06-29 17:25
modification date: Thursday 29th June 2023 17:25:41
---

**Tags:** #network #packets

#### Source:
[Packet](https://www.cloudflare.com/learning/network-layer/what-is-a-packet/)

--------------------------------------

### What it is:

* In networking, a packet is a small segment of a larger message
* Data sent over computer networks such as the internet, is divided into packets.
	* These packets are then recombined by the computer or device that receives them.

### Why use packets?

* Without doing packets we can transfer data between devices but there is some limitations like
	* We can transfer data between two devices without any issue if one more device came to network then it will be little hard
		* So on that time packet will play major role.
* Internet is [[Packet Switching]] network.

### What is packet loss?

* **What is hop count?**[](https://hopzero.com/what-does-hop-count-mean/)
	* Hop counter refers to the number of devices, usually routers, that a piece of data travels through.
	* Each time that a packet of data moves from one router to another then hop count will be counted as one.
	* Each count hop value will be reduced.
	* ttl is hop count.

* **Why HOP count is important?**
	* Some time packet will be not reached destination at that time packet is wasted on network, we can solve this issue by hop count.
	* If hop count hit 0 then packet will be destroyed
		* So user data will be safe
		* And packet switching process also stopped

* Occasionally, packets might bounce from router to router many times before reaching their destination IP address.
	* Enough of these kinds of lost data packets in the network can congest it, leading to poor performance.
	* Data packets that bounce around in the network too many times may get lost.
	* Hop count addresses this problem.

### What is a packet header?

* A packet header is a "label" of sorts, which provides information about the packet's contents, origin and destination.
* Packet consist of two portions
	* Header
		* It contains information about the packet, such as its origin and destination [[IP address]]
	* Payload
		* It is actual data.

### Where do packet headers come from?

* In practice, packets actually have more than one header, and each header is used by different part of the networking process. packet headers are attached by certain types of networking protocols.
* A protocol is a standardized way of formatting data so that any computer can interpret the data.
* Many different protocols make the internet work.
	* TCP/IP
	* OSI layer

### What is an IP packet?

* IP is a network layer protocol that has to do with routing. it is used to make sure packets arrive at the correct destination.
* Packets are sometimes defined by the protocol they are using.
* A packet with an IP header can be referred to as an IP Packet.


### What is network traffic?

* Network traffic is a term that refers to the packets that pass through a network, in the same way that automobile traffic refers to the cars and trucks that travel on roads.
* However, not all packets are good or useful, and not all network traffic is safe.
* Attackers can generate malicious network traffic data packets designed to compromise or overwhelm a network.
	* This can take the form of a [[DDoS Attack]] , a [[Vulnerability exploitation]] or several other forms of cyber attack.
