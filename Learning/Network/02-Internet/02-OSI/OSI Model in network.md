---
creation date: 2023-07-20 17:57
modification date: Thursday 20th July 2023 17:57:04
---

**Tags:** #network 

#### Source:
[OSI](https://www.cloudflare.com/learning/ddos/glossary/open-systems-interconnection-model-osi/)

--------------------------------------

### Explanation about it:

### What is the OSI model?

* OSI means Open systems interconnection model 
* It is a conceptual model created by the International organization for standardization 
	* Which enables diverse communication systems to communicate using standard protocols.
* OSI provides a standard for different computer systems to be able to communicate with each other.

![[Pasted image 20230720181152.png]]


### Why does the OSI model matter?

* OSI model will help to break down the problem and isolate the source of the trouble.


### 7 Layers of the OSI model?

#### 7. Application layer:

![[Pasted image 20230720185138.png]]

* This is the only layer that directly interact with data from the user.
* Software applications like web browsers and email clients rely on the application layer to initiate communication.
* Application layer is responsible for the protocols and data manipulation that the software relies on to present meaningful data to the user
* Some application layer protocol
	* [[HTTPS in network |HTTP]]
	* SMTP


#### 6. Presentation layer:

![[Pasted image 20230720185545.png]]

* Layer 6 makes the data presentable for application to consume.
* Also, it responsible for translation, encryption and compression of data.
* If the devices are communicating over an encrypted connection
	* Layer 6 is responsible for adding the encryption on the sender's end 
		* as well as decoding the encryption on the receiver's end so that it can present the application layer with unencrypted, readable data.
* Finally, presentation layer is also responsible for compressing data it receives from the application layer before delivering it to layer 5
	* This help improve the speed and efficiency of communication by minimizing the amount of data that will be transferred.

#### 5. Session layer

![[Pasted image 20230720190521.png]]

* This layer is responsible for opening and closing communication between the two devices.
* The time between when the communication is opened and closed is known as the session.
* session layer ensures that the session stays open long enough to transfer all the data being exchanged, and then promptly closes the session in order to avoid wasting resources.