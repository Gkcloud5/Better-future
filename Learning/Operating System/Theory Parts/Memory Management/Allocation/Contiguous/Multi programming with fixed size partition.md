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

* At a time CPU can only execute