#### Source:
[YT](https://www.youtube.com/watch?v=B5i-IAuYO6g&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=67)

* OS allocate frames to process by using 5 approach

#### 1. Equal allocation:

* Here frames will be allocated equally among available process.
	* p1 require 10 frames
	* P2 require 30 frames
	* Main memory has 40 frame

![[Pasted image 20230524153659.png]]

#### 2. Proportional allocation:

* Here frames should be allocated based upon size of a process
* Here priority won't be consider here

![[Pasted image 20230524153924.png]]

#### 3. Priority Allocation:

* Based upon priority frames will be allocated to a process

#### 4. Global replacement allocation:

* Whenever CPU is trying to execute a page, it check page is present in main memory or not
	* Suppose page is not present in main memory then it's called page fault.
	* 
	* 