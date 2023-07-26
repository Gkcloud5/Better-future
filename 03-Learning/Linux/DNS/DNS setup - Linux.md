---
creation date: 2023-06-15 16:59
modification date: Thursday 15th June 2023 16:59:35
---

**Tags:** #linux #kernel #DNS #network 

#### Source:
[LJ](https://linuxjourney.com/lesson/dns-setup)

--------------------------------------

#### Explanation about it:

* Some Popular DNS servers
	* BIND
	* DNSmasq
	* PowerDNS

##### BIND:

* It is most popular DNS server on the internet.
* BIND stands for Berkeley internet name domain.
* BIND responsible for translating human readable domain names into the numeric IP addresses that computers use to communicate with each other.

##### DNSmasq:

* Lightweight and much easier to configure than BIND. if you want simplicity and don't need all the bells and whistles of BIND, use DNSmasq.
* It comes with all the tools you need to setup DHCP and DNS, recommended for smaller network.

##### PowerDNS:

* Full featured and similar to BIND, it offers you little bit more flexibility with options. It reads information from multiple databases such as MySQL, postgreSQL, etc.