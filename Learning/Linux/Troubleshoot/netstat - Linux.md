---
creation date: 2023-06-15 13:46
modification date: Thursday 15th June 2023 13:46:46
tag: 
---

#### Source:
[LJ](https://linuxjourney.com/lesson/netstat)

--------------------------------------

#### Explanation about it:

* It something relate to port.
* to get list of ports
	* /etc/services

```
  
ftp             21/tcp
ssh             22/tcp
smtp            25/tcp   
domain          53/tcp  # DNS  
http            80/tcp
https           443/tcp 
..etc..
```

* First column is a name of the service then the port number and the transport layer protcol.

##### netstat:

* It very useful to get detailed information about your network.
* `netstat` displays various network related information such 
	* network connections
	* routing tables
	* information about network interfaces
* ##### Sockets and port:
	* A socket is an interface that allows programs to send and receive data while a port is used 