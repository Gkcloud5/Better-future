---
creation date: 2023-06-15 16:19
modification date: Thursday 15th June 2023 16:19:28
tag: 
---

#### Source:
[LJ](https://linuxjourney.com/lesson/dns-components)

--------------------------------------

#### Explanation about it:

##### Nameserver:

* We setup DNS via "nameservers"
* the nameserver load up our DNS settings and configs and answers any questions from clients or other servers that want to know things like "who is google.com" 
* If name server does not know the answer to that query, it will redirect the request to other nameservers.

##### Zone file:

* Inside a nameserver lives something called zone files.
* Zone files are how the name server stores information about the domain or how to get to the domain if it does not know.

##### Resource records:

* A zone file is comprised of entries of resource records.
* Each line is a record and contains information about hosts nameservers and other resources.
* Field consist of
	* Record name
	* TTL - The time after which we discard the record and obtain a new one. internet is constantly changing, one minute a host can be mapped to X IP address then next it can be at Y IP address.
	* Class - Namespace of the record information. most commonly IN is used for internet.
	* TYPE - Type of information stored in the record data.
		* A for address
		* MX or mail exchanger
	* Data - This field contain an IP address if it's an A record or something else depending on the record type.

