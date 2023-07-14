---
creation date: 2023-07-14 15:17
modification date: Friday 14th July 2023 15:17:59
---

**Tags:** #network #protocol

#### Source:
[BGP](https://www.cloudflare.com/learning/security/glossary/what-is-bgp/)

--------------------------------------

### What is BGP?

* Border gateway protocol is the postal service of the internet.
	* Someone submits data via the internet, BGP is responsible for looking at all of the available paths that data could travel and picking the best route
		* which usually means hopping between  [[Autonomous systems in network|AS]]
* BGP is the protocol that makes the internet work by enabling data routing.

### Difference between external BGP and internal BGP?

* Routers are exchanged and traffic is transmitted over the internet using the BGP.
* AS can also use an internal version of BGP to route through their internal networks, which is known as internal BGP.
* External BGP is like international shipping. there are certain standards and guidelines that need to be followed when shipping a piece of mail internationally.
	* Once that piece of mail reaches its destination country, it has to go through the destination country's local mail service to reach its final destination.

### BGP attributes?

* BGP tries to find most efficient path for network traffic.
* BGP assigns attributes to each path, 
	* And these attributes help routers select a path when there are multiple options. 
* Some example BGP attributes:
	* **Weight:** A cisco-proprietary attribute, this tells a router which local paths are preferred.
	* **Local preference:** This tells a router which outbound path to select.
	* **Originate:** This tells a router to choose router it added to BGP itself.
