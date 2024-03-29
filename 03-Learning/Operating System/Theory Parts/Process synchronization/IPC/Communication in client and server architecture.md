#### Source:
[YT](https://www.youtube.com/watch?v=AOrmV3NcBKU&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=14)
[Medium](https://medium.com/@subhangdxt/beginners-guide-to-client-server-communication-8099cf0ac3af)
[TP](https://www.tutorialspoint.com/operating-systems-client-server-communication#:~:text=Client%2FServer%20communication%20involves%20two,responds%20to%20the%20client%20requests.)

#### About Client/Server Communication:

* Client and server communication involves two components, namely client and a server.
* They are usually multiple clients in communication with a single server.
* The client send requests to the server and the server responds to the client requests.

![[Pasted image 20230514152544.png]]

* Communication in client/server architecture typically follows a request-response model. the client, which is usually a user interface or an application running on a user's device, initiates communication by sending a request to the server. the server which is a powerful machine, receives the request, processes it and generate response. the response is then sent back to the client.

##### Requests:
* Requests are sent from the client in order to ask the server for some data like files, or tell the server about things that happen, like that a user want to login with his credentials.

##### Response:
* A response is sent from the server to the client and is the reaction of the server to a request of the client. this could for example be an authentication result.

##### Service:
* A service is a specific task that the server provides for the client to use, like downloading image


#### Client server communication done in 3 ways:

1. [[Sockets]]
2. [[Remote procedure call]]
3. [[Pipes]]
