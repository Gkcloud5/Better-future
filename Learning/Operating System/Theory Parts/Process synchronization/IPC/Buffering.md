#### Source:
[YT](https://www.youtube.com/watch?v=fSMVWmGPqlM&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=13)

#### About Buffering:

* Buffering means what is a size of a buffer
* Buffer is a temporary storage area that is used to hold data while it is being transferred between different components or processes. 

##### 0 Capacity:
* It means there is a no buffer
* If sender send a message then sender has to wait until receiver receive a message because there is no space to hold next message

##### Finite Capacity:
* Finite means size of a buffer is limited

![[Pasted image 20230514150813.png]]

* If the buffer is full then sender has to wait till consumer consume a item from buffer

##### Infinite Capacity:
* Buffer size is infinite
* Here sender no need to wait till consumer consume data from buffer.
* Sender can put any number of buffer in this state