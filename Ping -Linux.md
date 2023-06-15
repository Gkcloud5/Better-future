---
creation date: 2023-06-15 13:32
modification date: Thursday 15th June 2023 13:32:48
tag: 
---

#### Source:
[LJ](https://linuxjourney.com/lesson/ping)

--------------------------------------

#### Explanation about it:

* It is used to test whether or not a packet can reach a host.
* It works by sending ICMP echo request packets to the destination host and waits for an ICMP echo reply (type 0).
	* Ping is successful when a host sends out the request packet and receives a response from the target.

```
root@root:~# ping -c 3 www.google.com
PING www.google.com (172.217.13.100) 56(84) bytes of data.
64 bytes from yul02s04-in-f4.1e100.net (172.217.13.100): icmp_seq=1 ttl=119 time=0.790 ms
64 bytes from yul02s04-in-f4.1e100.net (172.217.13.100): icmp_seq=2 ttl=119 time=0.744 ms
64 bytes from yul02s04-in-f4.1e100.net (172.217.13.100): icmp_seq=3 ttl=119 time=0.749 ms
```

* -c flag is used for count.
	* It stop sending echo request after the count has been reached.

##### icmp_seq:

* This is show the sequence of packets sent
	* In above example it have 3 packets.

##### ttl:

* Time to live field is used as a hop counter, as you make hops, it decrements a counter by one and once the hop counter reaches 0 then packet dies