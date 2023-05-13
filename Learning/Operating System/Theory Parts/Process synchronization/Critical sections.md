#### Source:
[YT](https://www.youtube.com/watch?v=QxXez-kiLf0&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=31)
[GFG](https://www.geeksforgeeks.org/g-fact-70/)
[JTP](https://www.javatpoint.com/os-critical-section-problem)

#### What is critical section:

* It is part of program where shared memory accessed
	* Shared file
	* Share memory
* In producer consumer problem example we will use a count variable to know buffer size value, If process try to accessing a count variable is known as critical section
	* Because producer when accessing a count variable it does not allow to access consumer, this thing will help to solve unwanted data corruption.
* Critical section is only one process at a time.

![[Pasted image 20230513191541.png]]

#### Ways to solve critical section:

1. Software solution
	1. Peterson's solution
2. Hardware solution
	1. Synchronization hardware

#### Solution for critical section problem need to satisfy 3 requirements:

##### 1. Mutual Exclusion:
* It means at a time only one process in critical section.
* When one process in critical section then another process should not be allowed in critical section.

##### 2. Progress:
* Let critical section does not have a process, some process in ready queue interested to enter in critical section then decision about which process enter into critical section, the decision should be taken in finite amount of time.