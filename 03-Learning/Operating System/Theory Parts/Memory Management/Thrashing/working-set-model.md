#### Source:
[YT](https://www.youtube.com/watch?v=v0QVLJFTAFs&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=69)

![[Pasted image 20230525094551.png]]

* Degree of multiprogramming means, placing more number of process in main memory.
* CPU utilization is good for some time after that when OS have more number of process in main memory is lead to slow down CPU process, it seems thrashing is occur.
* **Working-set-model,** works based on principle of locality or locality model.
	* locality of reference is over the short period of time as certain instruction executed repeatedly.
	* The working-set model works by tracking the pages that are most frequently used by a process. these pages are kept in memory.
		* While the pages that are not used as frequently are swapped out to disk
* working set of a process is resident in physical memory to minimize the frequency of page faults and the need for excessive disk I/O.