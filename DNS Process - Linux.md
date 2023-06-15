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
* 