---
creation date: 2023-07-20 17:57
modification date: Thursday 20th July 2023 17:57:04
---

**Tags:** #network 

#### Source:
[OSI](https://www.cloudflare.com/learning/ddos/glossary/open-systems-interconnection-model-osi/)
[YT](https://www.youtube.com/watch?v=Sn4nU7kSwEU)

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
* Session layer also synchronizes data transfer with checkpoints


#### 6. The transport layer:

![[Pasted image 20230721185104.png]]

* this layer is responsible for end-to end communication between the two devices.
* This includes taking the data from the session layer and breaking it up into chunks called segments before sending it to layer 3.
* The transport layer on the receiving device is responsible for reassembling the segments into data the session layer can consume.
* Transport layer is responsible for flow control and error control.
	* Flow control determines an optimal speed of transmission to ensure that a sender with a fast connection does not overwhelm a receiver with a slow connection
* Transport layer error control on the receiving end by ensuring that the data received is complete, and requesting transmission if it is not
* Protocols are
	* [[TCP in network]]
	* UDP


#### 3. The network layer:

![[Pasted image 20230721185733.png]]

* The network layer is a responsible for facilitating data transfer between two different networks
* If the two devices communicating are on the same network, then the network layer is unnecessary.
* The network layer breaks up segments from the transport layer into smaller units, called packets, on the sender's device.
	* And reassembling these packets on the receiving device.
* Also the network layer finds the best physical path for the data to reach its destination
* Protocols are
	* ICMP
	* IGMP
	* IPSec

#### 2. The data link layer:

![[Pasted image 20230721190225.png]]

* The data link layer is very similar to the network layer
* Except the data link layer facilitates data transfer between two devices on the same network.
* Data link layer takes packets from the network layer and breaks them into smaller pieces called frames.
* Data link layer also responsible for flow control and error control in intra network communication.

#### 1. Physical layer:

![[Pasted image 20230721191025.png]]

* This layer includes the physical equipment's in the data transfer, such as cables and switches.
* Here data gets converted into a bit stream
	* Which is a string 1's and 0's 
