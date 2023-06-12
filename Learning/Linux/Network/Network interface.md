---
creation date: 2023-06-12 10:54
modification date: Monday 12th June 2023 10:54:44
tag: 
---

#### Source:
[LJ](https://linuxjourney.com/lesson/network-interfaces)

--------------------------------------

#### Explanation about it:

* it is how the kernel links up the software side of the networking to the hardware side.

```
ifconfig -a
  
eth0      Link encap:Ethernet  HWaddr 1d:3a:32:24:4d:ce  
          inet addr:192.168.1.129  Bcast:192.168.1.255  Mask:255.255.255.0 
          inet6 addr: fd60::21c:29ff:fe63:5cdc/64 Scope:Link
```


##### ifconfig command:

* the ifconfig tool allows us to configure our network interfaces, if we don't have any network interfaces set up, the kernel device drivers and the network won't know how to talk to each others.
* ifconfig runs on bootup and configures our interfaces through config files, but we can also manually modify them.
* Output of ifconfig shows the interface nam