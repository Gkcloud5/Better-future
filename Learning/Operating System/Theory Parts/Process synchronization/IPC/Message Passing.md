#### About Message Passing:

![[Pasted image 20230514142810.png]]

![[Pasted image 20230514142847.png]]

* In order to sent message to another process, first need to sent message to kernel and then kernel will sent that message to destination process.

![[Pasted image 20230514143054.png]]


#### Issues while implementing message passing:

1. **[[Naming]]:**
 * How sender will send a message and how receiver will receive a message
	 * Direct communication
	 * Indirect Communication

2. **Synchronization**
 * How we will implement synchronization
	 * Blocked sender and Blocked receiver
	 * Non-Blocked sender and non blocked receiver

3. **Buffering**
 * What is a size of a buffer
	 * 0 capacity
	 * Finite capacity
	 * Infinite capacity

