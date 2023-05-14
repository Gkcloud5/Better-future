#### Source:
[YT](https://www.youtube.com/watch?v=AOrmV3NcBKU&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=14)

#### About Socket:
* It mainly useful to communication between two process
	* First process in client system
	* Destination process in server system
* Socket is combination of **IP address** and **Port number** 
	* EX: 102.34.56.11:80
* totally we have 1024 well defined port number
* Some protocol have defined port number that's are
	* FTP --> 21
	* HTTP --> 80

![[Pasted image 20230514162902.png]]

* Client machine will sent connection request to server with a help of socket. whenever server receive the connection request then it provide the corresponding repones to the client machine.
* If client request one more process then process will be have new port number.