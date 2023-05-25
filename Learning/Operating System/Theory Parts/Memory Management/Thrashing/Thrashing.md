#### Source:
[YT](https://www.youtube.com/watch?v=v0QVLJFTAFs&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=69)


* If a process spends more time on paging rather than executing then it's known as thrashing.
* Let consider p1 process needs 50 frame
	* But OS allocate 3 frames to process
	* So while executing P1 process it will have too many page fault occurs
	* More number of times swapping will occurs
	* Here swapping process is high when compare to executing process, so CPU will mostly idle.
* We have overcome thrashing by using following two methods
	* [[working-set-model]]
	* [[page-fault frequency]]