#### Source:
[YT](https://www.youtube.com/watch?v=JbmOegG9-J0&list=PL3uLubnzL2Tlbyrr2GFVRE7Azo8FJe-dJ&index=3)

**Process synchronization** --> **Interprocess Communication** --> **Message queue**

#### What is message queue:

* It is a one of the mechanism use to do Interprocess communication
* Messages are stored in a queue, and processes can send and receive messages from queue.
* [[Message Passing]]
* We are using 3 different system call for send message
	* msgsnd --> Will initialize queue
	* msgrcv --> will be used to receive the messages
	* mesgctl --> will be used for administrative privileges.
