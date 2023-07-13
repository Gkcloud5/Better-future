---
creation date: 2023-07-13 19:12
modification date: Thursday 13th July 2023 19:12:16
---

**Tags:** #network 

#### Source:
[NS](https://www.cloudflare.com/learning/network-layer/what-is-a-network-switch/)

--------------------------------------

### What is network switch?

* A network switch connects devices within a network and forwards data packets to and from those devices.
* Unlike a router, switch only sends data to the single device it is intended for, not to work multiple devices.

![[Pasted image 20230713191624.png]]



### What is the difference between a switch and a router?

* Routers are necessary for an internet connection
	* Routers select paths for data packets to cross networks and reach their destinations.
* Switches are only used for interconnecting devices.
	* Homes and small offices need routers for internet access.

### What is a layer 2 switch? what is layer 3 switch?

*  Network switches can operate at either OSI layer 2 or layer 3.
* Layer 2 switches forwarded data based on the destination MAC address, while layer 3 switches forward data based on the destination IP address. 
	* Some switches can do both.

### What is an unmanaged switch? what is a managed switch?

* An unmanaged switch simply creates more ethernet ports on a LAN.
	* So that more local devices can access the internet.
	* Unmanaged switches pass data back and forth based on device MAC addresses.
* Managed switch fulfills the same function for much larger networks, and offers network administrators much more control over how traffic is prioritized.
	* They also enable administrators to setup VLANs to further subdivide a local network into smaller chunks.

### What is the difference between a MAC address and an IP address?

* Network switches refer to MAC addresses in order to send internet traffic to the right devices, not IP addresses.
* Every device that connects to the internet has 
	* IP address
		* IP address are used at layer 3, which means computers and devices all over the internet use IP addresses for sending and receiving data.
	* MAC address
		* It is a permanent identifier for each piece of hardware, somewhat like a serial number.
		* MAC addresses are used at layer 2, not layer 3
			* Which means they are not included in IP packet headers.

**Layer 2 network switches maintain a table in memory that matches MAC addresses to the switch's ethernet ports. this table is called a content addressable memory table.**

