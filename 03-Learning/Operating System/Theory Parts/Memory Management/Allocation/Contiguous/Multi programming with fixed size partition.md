#### Source:
[YT](https://www.youtube.com/watch?v=7XOXQQFq5qw&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=51)


#### About it:

* This approach is contiguous memory allocation approach.
* Here, the number of partition are fixed, size of partition is same or different.
* Size of partition should be decided during system generation or system configuration.
* Once computer is designed with this approach then not possible to change later,

![[Pasted image 20230521150051.png]]

* Here, partition store only one process, even if it have free space it does not store any other process.

![[Pasted image 20230521150423.png]]

#### Advantage:

* It is very very easy to apply this approach.

#### Drawback:

##### Internal fragmentation:

* Partition also called fragmentation.
* If we lookup a 1st partition, we could see there is 2MB wasted, this wasted is called as internal fragmentation.
* in partition 2, 8MB is wasted.

##### Limitation on processes:

* At a time CPU can only execute how much partition count they have.
* If memory divided into 7 partition then CPU can execute only 7 process at a time.

##### Limitation on size of a process:

* Let consider if OS want to execute 100MB process, it's not possible, because partition maximum size is 25MB.

##### External fragmentation:

* Let consider OS have 20MB process size, when we look a memory totally we have around 23MB size but we can't allocate a those spaces to the process 
* Because they are already occupied with some other process so even if we have free space not able to assign a space to process.

##### Degree of multiprogramming:

* It's very less in this approach.

#### Memory allocation algorithm:

* ##### First fit:
	* consider we have 3 partition with a size of 10mb,20mb and 30mb.
	* allocate a first partition if it fit.
	* If we have a first process with size of 9MB, it check 1st partition 10mb then process will assigned.
	* OS 2nd process size is 25MB, it check 2nd partition with size of 20mb, size is very less when compare to process size so, it check next partition that size is 30MB so process will allocated that partition.
	* Last process is p3, while checking memory it find 2nd partition is free with 20mb so process will allocated there.

![[Pasted image 20230521152050.png]]

* ##### Best fit:
	* Allocate minimum partition that big enough for a process
	* Allocate a partition that's will have minimum fragmentation.
	* First, we have to scan all the free partition for this method
	* Let consider same example as we discussed above, but partition 2 size is 27MB, and 4th partition size is 17MB
		* Process 1 will be assigned to partition 1
		* Process 2 will be assigned in partition 2
		* process 3 will be assigned in partition 4

![[Pasted image 20230521152436.png]]


* ##### Worst Fit:
	* it is a opposite of best fit algorithm
	* maximum block will be assigned to corresponding process.
	* First, OS check all the free available partition size.
	* And, OS will assign 1st process to maximum partition size block