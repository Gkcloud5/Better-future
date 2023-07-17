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

* A lot of different kinds of hardware and infrastructure go into making the internet work for everyone.
	* [[Routers in network |Router]]
		* Forward packets to different computer network based on their destination.
		* Routers are like the traffic cops of the internet, making sure that internet traffic goes to the right networks

	* [[Network switch |Switch]]
		* Connect devices that share a single network. they use packet switching to forward packets to the correct devices.

        * [[Web servers in network | Web server]]
	        * It store and serve content to users.


### 5. How do these concepts relate to website and application users access over the internet?

* Packets are traveled over cables and radio waves and through routers and switches from our web server to your computer or device.
* Your computer or smartphone received those packets and passed them to your device's browser, and your browser interpreted the data within the packets in order to display the text you are reading now.

##### 5.1 Specific steps involved in this process:

###### 5.1 [[DNS in Networking |DNS query]]: 
* When your browser started to load this webpage, it likely first made a DNS query to find out the IP address.

###### 5.2 [[TCP Handshake]]
* Your browser opened a connection with that IP address.

###### 5.3 [[TLS Handshake]]
* Your browser also set up encryption between a  web server and your device so that attackers cannot read the data packets that travel between those two endpoints.

###### 5.4 [[HTTPS in network |HTTP]] request:
* Your browser requested the content that appears on this webpage.

###### 5.6 [[HTTPS in network |HTTPS]] response:
* Web server transmitted the content in the form of HTML, CSS and Javascript code, 
	* Broken up into a series of data packets.
	* Once your device received the packets and verified it had received all of them
	* Then your browser interpreted the HTML, CSS and Javascript code contained in the packets to render the content about the internet works.

##### 5.2 Some different processes and protocols are involved in loading webpage:

* [[DNS in Networking |DNS]]
* [[TCP in network |TCP]]
* [[TLS in networ |TLS]]
* [[HTTPS in network |HTTP]]

