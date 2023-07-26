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
	* A socket is an interface that allows programs to send and receive data while a port is used to identify which application should send or receive data. 
	* The socket address is the combination of the IP address and port.
	* Every connection between a host and destination requires a unique socket.

```
root@root:~# netstat -at
Active Internet connections (servers and established)
Proto Recv-Q Send-Q Local Address           Foreign Address         State
tcp        0      0 0.0.0.0:ssh             0.0.0.0:*               LISTEN
tcp        0      0 localhost:6010          0.0.0.0:*               LISTEN
tcp        0      0 localhost:domain        0.0.0.0:*               LISTEN
tcp        0      0 root:ssh                157.49.151.39:1263      ESTABLISHED
tcp        0    256 root:ssh                157.49.151.39:1256      ESTABLISHED
tcp6       0      0 [::]:ssh                [::]:*                  LISTEN
tcp6       0      0 ip6-localhost:6010      [::]:*                  LISTEN

```

* **Proto** - Protocol used, TCP or UDP
* **Recv-Q** - Data that is queued to be received
* **send-Q** - Data that is queued to be sent
* **Local Address** -  Locally connected host
* **Foreign Address** - Remotely connected host
* **State** - The state of the socket.

