#### Source:
[TP](https://www.tutorialspoint.com/unix/unix-communication.htm)

* communicate with remote users


#### ping utility:

* **ping** command sends an echo request to a host available on the network.
* Using this command, you can check if your remote host is responding well or not.
* ping command is useful for
	* Tracking and isolating hardware and software problems
	* Determining the status of the network and various foreign hosts
	* Testing, measuring and managing networks.

##### Syntax:

```
ping hostname or ip-address
```

##### Example:

```
ping google.com
PING google.com (74.125.67.100) 56(84) bytes of data.
64 bytes from 74.125.67.100: icmp_seq = 1 ttl = 54 time = 39.4 ms
64 bytes from 74.125.67.100: icmp_seq = 2 ttl = 54 time = 39.9 ms
64 bytes from 74.125.67.100: icmp_seq = 3 ttl = 54 time = 39.3 ms
64 bytes from 74.125.67.100: icmp_seq = 4 ttl = 54 time = 39.1 ms
64 bytes from 74.125.67.100: icmp_seq = 5 ttl = 54 time = 38.8 ms
--- google.com ping statistics ---
22 packets transmitted, 22 received, 0% packet loss, time 21017ms
rtt min/avg/max/mdev = 38.867/39.334/39.900/0.396 ms
```


#### ftp utility:

* ftp stands for File Transfer Protocol.
* This utility helps you upload and download your file from one computer to another computer
* This command help you perform tasks
	* Connect and login to a remote host
	* Navigate directories
	* List directory contents
	* put and get files

##### Syntax:

```
ftp hostname or ip-address
```

#### Important commands:

* **put filename**
	* Uploads filename from the local machine to the remote machine
* **get filename**
	* Download filename from the remote machine to the local machine
* **mput file list**
	* Uploads more than one file from the local machine to the remote machine.

![[Pasted image 20230601231154.png]]


#### telnet utility:

* Telnet is a utility that allows customer user at one site to make a connection, login and then conduct work on a computer at another site.