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
* Output of ifconfig shows the interface name on the left side and the right side shows detailed information.


```
#create an interface and bring it up

ifconfig eth0 192.168.2.1 netmask 255.255.255.0 up
```

```
#Bring up or down an interface
ifup eth0
ifdown eth0
```

##### ip command:

* ip command allows us to manipulate the networking stack of a system.

```
#show interface
ip link show

#show the statisticks of an interface
ip -s link show eth0

#show ip addresses allocated to interface
ip address show

#Bring interfaces up and down
ip link set eth0 up
ip link set eth0 down

#add an IP address to an interface
ip address add IPADDRESS/24 dev eth0
```


[[Route - Network - Linux]]

[[DHclient - Network - Linux]]




