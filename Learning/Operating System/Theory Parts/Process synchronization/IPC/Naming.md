#### Source:
[YT](https://www.youtube.com/watch?v=fSMVWmGPqlM&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=13)

### About Naming issue:

* Naming will specify how one process can send message to another process and how one process can receive message from another process.

#### Direct Communication:

* Here they use two operation
	* Send
	* Receive

##### Send:
* It is a system call
* Here explicitly need to mention receiver process name and message that we want to send to receiver process

##### Receiver:
* Wants to receive a message from another process
* Here it need to mention from name of which process they want to receive a message and message

![[Pasted image 20230514144808.png]]

#### Indirect Communication:

* Here process cannot communicate directly.
* Processes are use mediator to communicate with each other
* Mediator called as mail box
