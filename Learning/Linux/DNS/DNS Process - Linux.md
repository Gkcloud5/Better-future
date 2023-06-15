---
creation date: 2023-06-15 16:40
modification date: Thursday 15th June 2023 16:40:48
tag: 
---

#### Source:
[LJ](https://linuxjourney.com/lesson/dns-process)

--------------------------------------

#### Explanation about it:

* It's an example of how your host finds a domain with DNS.
* We funnel our way down until we reach the DNS server that know of that domain

##### Local DNS server:

* First our host asks, "where is domain?", our local DNS server doesn't know so it goes and starts from the top of the funnel to ask the root servers.

##### Root servers:

* There are 13 root servers for the internet, they are mirrored and distributed around the world to handle DNS requests for the internet.
* So there are really hundreds of servers that are working, they are controlled by different organizations and they contain information about
	* Top-level domain
* Top level domain is .org, .com, .net, etc..
* So if domain have .com then the root server tell check IP address in .com top level domain DNS server.

##### Top-level domain:

* we send another request to the name server that knows ".com" addresses and asks if it knows where "domain.com is?"
	* TLD doesn't have the domain.com in their zone files, but it does see a record 