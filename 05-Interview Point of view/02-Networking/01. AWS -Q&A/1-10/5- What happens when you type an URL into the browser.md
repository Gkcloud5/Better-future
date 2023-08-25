
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

#### What is DNS(Domain Name System)?

* DNS stores data that used to mapping from domain name to IP address.
* Hard to remember a IP address that's the reason for we use domain name.
* Each domain name have unique IP address.
* Client get IP address by using DNS.