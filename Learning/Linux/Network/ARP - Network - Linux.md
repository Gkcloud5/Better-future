---
creation date: 2023-06-13 22:18
modification date: Tuesday 13th June 2023 22:18:27
tag: 
---

#### Source:
[LJ](https://linuxjourney.com/lesson/arp-command)

--------------------------------------

#### Explanation about it:

* It checks locally stored ARP cache on our system.

```
arp
Address                  HWtype  HWaddress           Flags Mask            Iface 
192.168.22.1            ether   00:12:24:fc:12:cc   C                     eth0  
192.168.22.254          ether   00:12:45:f2:84:64   C                     eth0
```

* ARP stands for address resolution protocol. it is a protocol used in computer networks to resolve or map an IP address to mac address.
* ARP cache is actually empty when a machine boots up, it gets populated as packets are being sent to other hosts.
* If we sent a packet to a destination that is not in the ARP cache, the following happens
	* Source host create the ethernet frame with an ARP request packet
	* Source host broadcasts this frame to the entire network
	* If one of the hosts on the network knows the correct MAC address, it will send a reply packet and frame containing the mac address.
	* The source host adds the IP to MAC address mapping to the ARP cache and then proceeds with sending the packet.