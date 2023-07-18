---
creation date: 2023-07-17 21:37
modification date: Monday 17th July 2023 21:37:30
---

**Tags:** #network #protocol 

#### Source:
[CF](https://www.cloudflare.com/learning/ddos/glossary/tcp-ip/)

--------------------------------------

### Explanation about it:

#### What are IP and TCP?

* The [[Internet protocol in networking |IP]] is the address system of the internet and has the core function of delivering packets of information from source device to a target device.
* IP does not handle packet ordering or error checking. Such functionality requires another protocol, that is **Transmission control Protocol**
* TCP/IP relation is, packets travel through different router, some of packet take longer than others, 
	* When packets arrive after traversing their different paths, the pieces may be out of order.
	* IP make sure the pieces arrive at their destination address.
	* TCP can be thought of a packet assembler on the other side. who puts the pieces together the right order, asks for wrong pieces to be resent, and let the sender know the packets has been received.
	* TCP maintain connection with sender till the last packet receive
* IP is a connectionless protocol, which means that each unit of data is individually addressed and routed from the source device to target device.
	* Target does not send an acknowledgement back to the source, that's where protocol such as TCP come in.
		* TCP is used in conjunction with IP in order to maintain a connection between the sender and the target and to ensure packet order.
