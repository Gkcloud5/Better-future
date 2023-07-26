---
creation date: 2023-07-24 17:35
modification date: Monday 24th July 2023 17:35:04
---

**Tags:** #network 

#### Source:
[CDN](https://www.cloudflare.com/learning/cdn/what-is-a-cdn/)
[YT](https://www.youtube.com/watch?v=RI9np1LWzqw)

--------------------------------------

### Explanation about it:

### What is a CDN?

* A Content Delivery Network is a geographically distributed group of servers that caches content close to end users.
* CDN allows for the quick transfer of assets needed for loading internet content, including HTML pages, JS files, CSS 
* It also help protect website against some common malicious attacks, such as
	* DDoS
* Bring servers close to the used


#### Is a CDN the same as a web host?

* While a CDN does not host content
* And can't replace the need for proper web hosting
* It does help [[Cahce in network |Cache]] content at the [[Network Edge in networing | Edge network]]
	* Which improves website performance


#### Benefits of using CDN?

##### Improving website load times:
* Distributing content closer to website by using a nearby CDN server,
	* Visitors experience faster page loading times.
* CDN can reduce bounce rates and increase the amount of time that people spend on the site.

##### Reducing bandwidth costs:
* Through caching and other optimizations
	* CDN are able to reduce the amount of data an origin server must provide,
		* Thus reducing hosting costs for website owners


#### How does a CDN work?

* a CDN is a network of servers linked together with the goal of delivering content as quickly, cheaply, reliably and securely as possible.
* a CDN will place servers at the exchange point between different networks
* [[Internet exchange point]] are the primary locations where different internet providers connect in order to provide each other access to traffic originating on their different networks.

![[Pasted image 20230725170932.png]]


#### How does CDN improve website load times?

* It reduce  distance between users and websites resources. 
	* Instead of having to connect to website [[Origin server]], a CDN lets user connect to a geographically close [[data center in networking |Data center]].
		* Less travel time means faster service
* Hardware and software optimizations such as efficient  load balancing and solid state hard drives can help data reach the user faster
* CDN can reduce the amount of data that's transferred by reducing file sizes.
* CDN can also speed up sites which use TLS/SSL certificates by optimizing connection reuse and enabling TLS false start.

