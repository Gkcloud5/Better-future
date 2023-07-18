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
	* TCP can be thought of a packet assembler on the other side 