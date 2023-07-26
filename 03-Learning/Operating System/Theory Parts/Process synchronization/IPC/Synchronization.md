#### Source:
[YT](https://www.youtube.com/watch?v=fSMVWmGPqlM&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=13)


#### About synchronization:

##### Blocked sender and Blocked receiver:

* It is a synchronization
* **Blocked Sender:** If sender sent a message then sender will be blocked until the receiver receive a message. 
	* If receiver have some other work then during that time sender will be blocked once the receiver received a message then sender will be unblocked and able to send next message
* **Blocked Receiver:** Receiver process must be blocked until the sender get message from receiver

##### Non-Blocked sender and non blocked receiver:

* It is a asynchronization method
* **Non-Blocked sender:** If sender send a message then it does not worry about if message received by receiver or not they can continue their work message sending.
* **Non-Blocked receiver:** it is busy with it's own work
