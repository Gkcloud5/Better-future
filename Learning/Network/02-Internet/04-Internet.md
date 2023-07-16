---
creation date: 2023-07-15 18:36
modification date: Saturday 15th July 2023 18:36:17
---

**Tags:** #network #internet 

#### Source:
[CF](https://www.cloudflare.com/learning/network-layer/how-does-the-internet-work/)

--------------------------------------

#### Explanation about it:

### What is the internet?

* **About network:**
	* A network is a group of connected computers that are able to send data to each other.

* The internet is a vast, sprawling collection of networks that connect to each other.
	* Interconnected networks.

* Since computers connect to each other within networks and these networks also all connect with each other, one computer can talk to another computer in a faraway network thanks to the internet.
	* This makes it possible to rapidly exchange information between computers across the world.


### What is distributed networking?

* There is no control center for the internet.
	* It is distributed networking system.
* The internet's distributed nature makes it resilient.
	* Computers, servers and other pieces of networking hardware connect and disconnect from the internet all the time without impacting how the internet functions.


### 3. How does the internet work?

* Two main concepts that are fundamentals way the internet functions
	* Packets
	* Protocols

##### 3.1 Packets:

* A packet is a small segment of a larger message.
	* Each packet contains both data information about that data.
* [[Data packets]]
* Packets are sent across the internet using technique called [[Packet Switching]]

##### 3.2 Protocol:

* Generally, computers are have different type configuration so we are using some protocol to communicate a device that connected in network.
* In networking, a protocol is a standardized way of doing certain actions and formatting data so that two or more devices are able to communicate with and understand each other.
* These are the protocol sending packets between devices on the same network
	* For sending packets from network to network [[Internet protocol in networking|IP]]
	* For ensuring those packets successfully arrive in order [[TCP in network |TCP]]
	* And for formatting data for websites and applications are [[HTTPS in network|HTTPS]]
	* In addition to these foundational protocols, these are
		* Protocols for routing
		* Testing
		* encryption
	* Some alternative protocol we have, like for streaming video often we use [[UDP in network|UDP]] instead of TCP.


### 4. What Physical infrastructure makes the internet work?
