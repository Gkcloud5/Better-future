#### Source:
[YT](https://www.youtube.com/watch?v=mw6lfS6A6Bs&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=52)

#### About it:

* MVT -> Multiprogramming with variable size 
* This is a one of the contiguous memory location approach.
* Here partition count is depends upon number of process
	* If OS have 50 process then it should have 50 partition and size of partition is depends on size of a process.

![[Pasted image 20230522120318.png]]

#### Advantage:

* There is no internal fragmentation
* There is no limitation on number of partitions.
* There is no limitation on size of a process.

#### Drawback:

* It is difficult to apply this approach.
* External fragmentation:
	* If we have free box in ram not in order so one process not able to assign those free box if size is not matched.
	* We can solve this issue by using compaction
		* Combining free box and allocate it to process.
