#### Source:
[YT](https://www.youtube.com/watch?v=0u4ZyblK_YY&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=38)
[GFG](https://www.youtube.com/watch?v=0u4ZyblK_YY&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=38)
[JTP](https://www.javatpoint.com/os-deadlocks-introduction)

#### What is deadlock:

* Main task of OS is allocate resources to process.
* Deadlock is a state in OS where two or more processes are unable to process because each is waiting for a resource held by another process.
* In other words, it's a situation where two or more processes are indefinitely blocked, unable to complete their execution.
* Mostly it happens when processes need to access shared resources, such as memory or files.

#### Example for deadlock:

* Let consider dinning philosophers problem
* Philosophers are sitting around the table with bowls of rice and chopsticks
	* Each philosopher needs two chopsticks to eat their meals
* Following scenario lead to **deadlock**
	1. All philosophers pick up the chopstick on their right simultaneously.
	2. Each philosopher now wait for the chopstick on their left to be available.
	3. since every philosopher waiting for another philosopher to put chopstick down on table, none of them can proceed and eat their meal.
	4. The system reaches a deadlock state, and the philosophers remain indefinitely blocked.

#### Things we know in above example:

* Mutual exclusion
* Hold and wait
* no preemption
* circular wait

These conditions together lead to a situation where processes cannot make progress, resulting a deadlock.

#### Topics:

1. [[Deadlock detection and recovery]]
2. 