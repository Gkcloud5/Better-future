#### Source:
[GFG](https://www.geeksforgeeks.org/multilevel-queue-mlq-cpu-scheduling/)
[YT](https://www.youtube.com/watch?v=gm7y51393oE&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=28)

#### What is MLQ scheduling:

* Here one ready queue process are divided to multiple ready queue.
* For example, a ready queue converted to 4 parts
	* System process --> OS related process --> very very important
	* Foreground process --> Process response time is very very less
	* Background process --> process response time is not matter, not much important type process
	* Student process --> If we develop any program
* Based on process characteristic, it will assign as per the queue
* in above thing each queue will be different scheduling algorithm.
* How we can schedule to different queue
	* Fixed preemptive priority scheduler
	* time slicing between queue