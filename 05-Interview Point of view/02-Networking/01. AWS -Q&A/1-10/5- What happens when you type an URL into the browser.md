
### Resources:
1. [SD](https://systemdesign.one/what-happens-when-you-type-url-into-your-browser/)
2. [FC](https://www.freecodecamp.org/news/what-happens-when-you-hit-url-in-your-browser/)

### Major operations that happening while URL loading:

1. DNS resolution
2. TCP - Three way handshake
3. HTTPS Upgrade
4. HTTP Request/Response
5. Browser rendering

#### Terminology:
* **DNS:** Data store that contains the mapping from domain name to IP address
* **HTTP:** Standard application level protocol used to exchange files on the internet
* **HTTPS:** Secure version of HTTP
* **TCP:** Standard that defines how to establish and maintain a network conversation between a client and server
	* **Client:** Web browser or mobile device
	* **Server:** A computer that stores files and information in the form of a website
* **URL:** Web address to identify a web resources

### Introduction:
* Client must find a IP address of server to load a requested content.

![[Pasted image 20230825161001.png]]

### 1. What is DNS(Domain Name System)?

* DNS stores data that used to mapping from domain name to IP address.
* Hard to remember a IP address that's the reason for we use domain name.
* Each domain name have unique IP address.
* Client get IP address by using DNS.
* DNS have hierarchy approach

![[Pasted image 20230825161325.png]]

* DNS resolution starts at the root domain, TLD and works its way down to the second level domain.
* URL consists of the following parts:
	* Protocol
	* Subdomain
	* Domain
	* Top-level domain

![[Pasted image 20230825161509.png]]

##### Operations executed in sequential order for DNS resolution:

![[Pasted image 20230825161725.png]]

1. Browser(Clients) checks if the hostname IP address mapping exists in the local cache of the client.
2. If the last step failed, Clients check OS local cache by executing system call
3. If above step failed, Client makes a DNS request to the router and check the local cache of the router
4. If last step failed, Router forwards the request to the ISP and checks the DNS cache of the ISP.
5. If above step failed, DNS resolver queries the root servers(13 root servers)
6. DNS resolver queries TLD servers such as .com, .org
7. DNS resolver queries authoritative name servers such as google.com
8. Optionally, DNS resolver queries authoritative subdomain servers such as maps.google.com depending on the query

![[Pasted image 20230825162326.png]]

* Once the DNS query resolved, DNS resolution process would cache the result with a TTL expiry time limit.
* Cache improves the latency of subsequent client requests

### 2.[[Three way handshake - TCP|TCP Three-way handshake:]]

* Client should create a connection the server to transfer and receive data.
* TCP protocol used to do that stuf.
* Client perform three way handshake with server to establish TCP connection.
	* Bi-directional so 3 way
	* If single directional then 2 way is enough
![[Pasted image 20230825162805.png]]

* **SYN** and **ACK** messages are sent between the client and the server to open a TCP connection:
	* Clients sends an SYN request with a random sequence number
	* Server responds SYN+ACK. acknowledgement number is set to one more than the received sequence number. 
		* Server sends another random sequence number(y)
	* Client sends ACK. clients sends an acknowledgement number that is one more than the received sequence number.

### 3. [[HTTPS in network|HTTPS Upgrade]]

* 