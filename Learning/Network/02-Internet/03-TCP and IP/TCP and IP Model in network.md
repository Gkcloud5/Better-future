---
creation date: 2023-07-23 17:58
modification date: Sunday 23rd July 2023 17:58:15
---

**Tags:** #network 

#### Source:
[TCP](https://www.techtarget.com/searchnetworking/definition/TCP-IP)

--------------------------------------

### Explanation about it:

#### What is TCP/IP:

* It stands for transmission control protocol
* It used to interconnect network devices on the internet.
* TCP/IP is also used as communication protocol in a private computer network.
* TCP/IP specifies how data is exchanged over the internet by providing end-to-end communication that identify how it should be broken into packets, addressed, transmitted, routed and received at the destination.
* Two main protocol is
	* TCP
		* It defines how application can create channels of communication across a network.
		* It also manages how a message is assembled into smaller packets before they are then transmitted over the internet.
		* And reassembled in the right order.
	* IP
		* It defines how to address and route each packet to make sure it reach right destination.

##### Common TCP/IP protocol:
* HTTP 
	* Handles communication between a web server and a web browser
* HTTPS
	* Handles secure communication between a web server and a web browser
* FTP
	* It handles transmission of file between computers

#### How does TCP/IP work?

* It used client-server model of communication
* It is classified as stateless
	* It means client request is considered new because it is unrelated to previous request
	* It's not going to store any data

#### Why TCP/IP important?

* It is highly scalable and as a routable protocol
* It can determine the most efficient path through the network.
* Also it controlled by any company.

#### Layers in TCP/IP:[](https://www.javatpoint.com/computer-network-tcp-ip-model)

##### 1. Application layer:
* It provides application with standardized data exchange
* Protocols used
	* HTTPS
	* FTP
	* SMTP
* It is responsible for handling high-level protocols
* This layer allows the user to interact with the application.
* When one application layer protocol wants to communicate with another application layer, it forwards its data to the transport layer.

##### 2. Transport layer:
* 