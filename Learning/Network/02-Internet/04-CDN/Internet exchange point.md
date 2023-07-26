---
creation date: 2023-07-25 18:24
modification date: Tuesday 25th July 2023 18:24:36
---

**Tags:** #network 

#### Source:
[IEP](https://www.cloudflare.com/learning/cdn/glossary/internet-exchange-point-ixp/)

--------------------------------------

### Explanation about it:

#### What is an internet exchange point?

* IXP is a physical location through which internet infrastructure companies such as ISP and CDN's connect with each other.
* This location exist on the "edge" of different networks.
* By having a presence inside of an IXP location, companies are able to shorten their path to transit coming from other participating networks
	* Thereby reducing latency, improving round-trip time and reduce cost also.
* IXP is a physical location where multiple ISP, content providers and other network operators come together to exchange internet traffic between their networks.
* Main purpose of IXP is to vacillate the direct exchange of data traffic instead of routing it though 3rd party networks.
	* It will improve efficiency, speed and cost effectiveness

#### How does an IXP work?

* An IXP is essentially one or more physical locations containing network switches that route traffic between the different members networks
* IXP are large layer 2 LAN's that are built with one or many ethernet switches interconnected together across one or more physical buildings.


#### Why are IXP important?

* Traffic going from one network to another would potentially rely on an intermediary network to carry the traffic from source to destination, these are called transit providers.
* In large portion of international internet flows is cost prohibitive to maintain direct connection
* A CDN with IXP presence has the the advantage of optimizing the path through which data flows within it's network, cutting down on inefficient paths.


#### How do providers share traffic across different networks?

##### Transit:
* Agreement between a customer and it's upstream provider.
* A transit provider provides its customers with full connectivity to the rest of the internet.
* BGP protocol is used to allow customer IP addresses to be announced towards the transit provider and then onwards the rest of the global internet.

##### Peering:
* arrangement behind how networks share IP addresses without an intermediary between them.
* when traffic is transferred for free from one network to the next, the relationship is called settlement-free peering.