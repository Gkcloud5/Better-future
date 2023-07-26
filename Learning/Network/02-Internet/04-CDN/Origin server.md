---
creation date: 2023-07-26 17:25
modification date: Wednesday 26th July 2023 17:25:13
---

**Tags:** #network  

#### Source:
[OS](https://www.cloudflare.com/learning/cdn/glossary/origin-server/)

--------------------------------------

### Explanation about it:

### What is an origin server?

* Purpose of an origin server is to process and respond to incoming internet requests from internet clients.
* Concept of origin server is typically used in conjunction with the concept of an edge server or caching server.
* An origins server can take on all the responsibility of serving up the content for an internet property such as a website.
* Physical distance between origin server and a client making a request adds latency to the connection.


##### What is the difference between an origin server and a CDN edge server?

* CDN edge servers are very important in internet provider in location across the globe in order to deliver content as quickly as possible.
* A edge server lives inside a CDN on the edge of a network, 
	* And it's specifically designed to quickly process requests.
* Edge server's cache content like HTML, CSS and JS as close as possible to requesting machine.
* **Origin servers** still have an important server-side code such as the database of hashed client credentials used for authentication it typically maintained inside an origin server.
