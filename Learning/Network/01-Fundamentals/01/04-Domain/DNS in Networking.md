---
creation date: 2023-07-05 21:38
modification date: Wednesday 5th July 2023 21:38:33
---

**Tags:** #network 

#### Source:
[DNS](https://www.cloudflare.com/learning/dns/what-is-dns/)

--------------------------------------

### What it is:

* **Domain Name System**
* It is the phonebook of the internet.
* DNS translates domain names to IP addresses so browsers can load internet resources.

### How does DNS work?

* The process of DNS resolution involves converting a hostname into a computer friendly IP address.
* 4 DNS servers involved in loading a webpage
	* DNS recursor
	* Root nameserver
	* TLD nameserver
	* Authoritative nameserver



![[Pasted image 20230706164847.png]]


##### DNS recursor:

* The DNS recursor is a server designed to receive queries from client machines through application such as web browsers.
* Typically the recursor is then responsible for making additional requests in order to satisfy the client's DNS query.


##### Root nameserver:

* The root server is the first step in translating human readable host names into IP address.

![[Pasted image 20230706165328.png]]

