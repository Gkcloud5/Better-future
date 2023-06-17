---
creation date: 2023-06-16 16:06
modification date: Friday 16th June 2023 16:06:42
---

**Tags:** 

#### Source:
[YT](https://www.youtube.com/watch?v=6Ra17Qpj68c)

--------------------------------------

#### Explanation about it:

![[Pasted image 20230616160712.png]]

* **Net filter:** It is a firewall framework.
* Iptable is utility to control and manage net filter.
* Table is collection of chain
	* Filter table
	* Nat table
	* Mangle table
* Filter table:
	* Filtering incoming and outgoing traffic
* Nat table:
	* Redirect connection to other interface on network
* Mangle table:
	* Modifying particular packet and connection.


##### Chains:

* Chains can be seen as tags that define and match packets to the state
* **Input chain:** It is used to manage incoming packets and connection's and to a particular service to a protocol.
* **Output Chain:** It is used to manage outgoing packets after they have been created or processed.
* **Forward chain:** It is used to forward incoming packets from their source to the destination.

**Firewall rules is a responsible for managing a input and output of packets of server**

##### Target:

* What going to happen if packet match with firewall rule
	* Accept
	* Reject
	* Drop


```
#to view rules
iptables -L

#set rule
iptables --policy INPUT ACCEPT

#to delete rule
iptables -L --line-numbers
iptables -D INPUT *linenumber*

#
``` 