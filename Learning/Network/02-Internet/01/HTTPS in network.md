---
creation date: 2023-07-18 17:21
modification date: Tuesday 18th July 2023 17:21:49
---

**Tags:** #network 

#### Source:
[CF](https://www.cloudflare.com/learning/ddos/glossary/hypertext-transfer-protocol-http/)

--------------------------------------

### Explanation about it:

### 1. What is HTTP:

* Hypertext Transfer Protocol
* It is the foundation of the WWW, and is used to load webpages using hypertext links.
* HTTP is an **Application Layer** protocol
	* Designed to transfer information between networked devices 
		* And runs top of other layers of the network protocol stack.
*  A typical flow over HTTP involves a client machine making a request to a server, which then sends a response message.


### 2. What is in an HTTP request?

* An HTTP request is the way internet communication platforms such as web browsers ask for the information they need to load website.
* Each HTTP request made across the internet carries with it a series of encoded data that carries different types of information.
* HTTP request contains
	* HTTP version type
	* a URL
	* an HTTP method
	* HTTP request headers
	* Optional HTTP body.

##### 2.1 What is an HTTP method?

* An HTTP method, sometimes referred to as an HTTP verb
	* Indicates the action that the HTTP request expects from the queried server.
	* Most common HTTP methods are
		* GET 
			 * It expects information back in return
		* POST
			* It request typically indicates that the client is submitting information to the web server.
			* Such as submitting information.


##### 2.2 What are the HTTP request headers?

* HTTP headers contain text information stored in key value pair
* They are included in every HTTP request (and response).
* This headers communicate core information, such as what browser the client is using and what data is being requested.
* Example

![[Pasted image 20230718191547.png]]


##### 2.3 What is in an HTTP request body?

* Body of the request is the part that contains the body of information the request is transferring.
* Body contains any information being submitted to the web server, such as a username and password, or any other data entered into a form.

##### 2.4 What is in an HTTP response?

* An HTTP response is what web clients receive from an internet server in answer to an HTTP request.
* Typical HTTP response contains
	* HTTP status code
	* HTTP response headers
	* optional HTTP body.

##### 2.4.1 What's an HTTP status code?

* It's 3 digit code most often used to indicate HTTP request has been successfully completed.
	* 1xx informational
	* 2xx success
	* 3xx Redirection
	* 4xx Client error
	* 5xx Server Error
	* xx refers to different numbers between 00 and 99

##### 2.4.2 What are HTTP response headers?

* HTTP response comes with headers that convey important information such as the language and format of the data being sent in the response body. 

![[Pasted image 20230720174614.png]]


##### 2.4.3 What 