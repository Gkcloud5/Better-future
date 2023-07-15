---
creation date: 2023-07-15 13:36
modification date: Saturday 15th July 2023 13:36:12
---

**Tags:** 

#### Source:
[CG]()(https://chat.openai.com/share/ed020e5f-07c5-4e32-b966-db0fd844e37b)

--------------------------------------

#### Explanation about it:

* It is a type of routing algorithm used in computer networks to determine the best path for data packets to travel from source to destination.
* It's operates based on the exchange of information among network nodes. 
	* Each node gathers information about the state of its directly connected links and shares this information with other nodes in the network.

### Working overview:

##### Discovery:
* Each node in the network initially discovers its neighboring nodes and determines the cost associated with each link.
	* This information is typically obtained through a process called link state advertisement exchange.

##### Building a link state database:
* Each node collects the LSAs received from neighboring nodes and builds a comprehensive database that represents the cur