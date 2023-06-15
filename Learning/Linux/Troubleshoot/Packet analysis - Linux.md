---
creation date: 2023-06-15 15:29
modification date: Thursday 15th June 2023 15:29:29
tag: 
---

#### Source:
[LJ](https://linuxjourney.com/lesson/packet-analysis)

--------------------------------------

#### Explanation about it:

* Two popular packet analyzers
	* Wireshark
	* tcpdump
* These tools scan your network interfaces and capture the packet activity, parse the packages and output the information for us to see.

```
apt install tcpdump

tcpdump -i eth0
tcpdump: verbose output suppressed, use -v[v]... for full protocol decode
listening on eth0, link-type EN10MB (Ethernet), snapshot length 262144 bytes
10:10:30.119058 IP root.ssh > 157.49.151.39.1256: Flags [P.], seq 3049165798:3049165974, ack 333507524, win 717, length 176
10:10:30.148966 IP 157.49.151.39.1256 > root.ssh: Flags [.], ack 4294966912, win 254, length 0
10:10:30.158908 IP 157.49.151.39.1256 > root.ssh: Flags [.], ack 4294967024, win 254, length 0
10:10:30.168973 IP 157.49.151.39.1256 > root.ssh: Flags [.], ack 4294967120, win 254, length 0
10:10:30.201034 ARP, Request who-has 38.102.86.82 tell _gateway, length 46
10:10:30.248947 IP 157.49.151.39.1256 > root.ssh: Flags [.], ack 4294967168, win 253, length 0
10:10:30.301116 ARP, Request who-has 38.102.86.80 tell _gateway, length 46
10:10:30.358973 IP 157.49.151.39.1256 > root.ssh: Flags [.], ack 0, win 253, length 0
10:10:30.401659 ARP, Request who-has 38.102.86.81 tell _gateway, length 46
10:10:30.439015 IP 157.49.151.39.1256 > root.ssh: Flags [.], ack 176, win 252, length 0
10:10:30.701085 ARP, Request who-has 38.102.86.122 tell _gateway, length 46
10:10:30.801681 ARP, Request who-has 38.102.86.126 tell _gateway, length 46
10:10:30.889070 IP root.ssh > 157.49.151.39.1256: Flags [P.], seq 176:256, ack 1, win 717, length 80
10:10:30.890619 IP root.ssh > 157.49.151.39.1256: Flags [P.], seq 256:352, ack 1, win 717, length 96
10:10:30.891916 IP root.ssh > 157.49.151.39.1256: Flags [P.], seq 352:432, ack 1, win 717, length 80
10:10:30.892329 IP root.ssh > 157.49.151.39.1256: Flags [P.], seq 432:480, ack 1, win 717, length 48
10:10:30.893278 IP root.ssh > 157.49.151.39.1256: Flags [P.], seq 480:544, ack 1, win 717, length 64

```

