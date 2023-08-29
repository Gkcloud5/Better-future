
[Medium](https://medium.com/networks-security/computer-communication-locally-and-remotely-13d68f29efbc)


#### Communication via TCP/IP network:

* `ipconfig` command will show following information
	* Physical Address of your device (MAC).
	* IP address along with subnet mask.
	* Default Gateway (Router assigned for sending IP packets)
	* DNS Server IP

![[Pasted image 20230829152346.png]]

* Computer A wants to talk to B and C. The Computer A uses its subnet mask to find out if B and C are local or remote.
* Then to communicate locally with B, A follows:
	* Step1: A asks for B's MAC address using ARP
	* Step2: B replies to A with its MAC address
	* Step3: A uses frames to communicate with B
* All Communication between A and B would require a switch (layer 2 device). default gateway(layer 3 device) will not be used in this case.

Now, let's see how A talks with C:
* Step1: A asks for the MAC address of the default gateway using ARP.
* Step2: The default gateway replies to A with its MAC address.
* Step3: A sends its IP packets to the default gateway, which delivers the message of A to C.

#### Via wired connections:
* **Ethernet:**
	* Devices can communicate over Ethernet cables using TCP/IP protocols.
	* This is commonly used for networking computers, printers and other devices in a LAN.
* **USB:**
	* USB connections allow devices to exchange data directly via USB cables.

#### Via Wireless Connections:
* 
