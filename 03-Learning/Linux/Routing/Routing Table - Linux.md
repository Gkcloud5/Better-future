---
creation date: 2023-06-08 21:24
modification date: Thursday 8th June 2023 21:24:07
tag: 
---

#### Source:
[LJ](https://linuxjourney.com/lesson/routing-table)

--------------------------------------

#### Explanation about it:

```
route -n

Kernel IP routing table
  
Destination     Gateway         Genmask         Flags Metric Ref    Use Iface 
0.0.0.0         192.168.224.2   0.0.0.0         UG    0      0        0 eth0
192.168.224.0   0.0.0.0         255.255.255.0   U     1      0        0 eth0
```

##### Destination:

* In this field, we have a destination IP address of 192.168.224.0, this says that any packet that tries to go to this network.
* If address is in 0.0.0.0, it seems routing table does not know where that goes, so it denotes it, and therefore routes our packet to the gateway.

##### Gateway:
* If we are sending a packet that is not on the same network, it will be sent to this gateway address.

##### Genmask:
* This is the subnet mask, used to figure out what IP addresses match what destination.

##### Flags:

* UG - Network is Up and is a gateway.
* U - Network is UP.

##### iface:
* This is the interface that our packet will be going out of, eth0 usually stands for the first ethernet device on your system.