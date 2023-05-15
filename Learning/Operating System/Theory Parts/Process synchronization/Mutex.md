#### Source:
[YT](https://www.youtube.com/watch?v=z7Oev-s4m8M)


#### About Mutex:

* Mutex is a synchronization primitive used to control access a shared resources by multiple thread or processes.
* It's purpose to prevent multiple threads from accessing shared data simultaneously. which could lead to data inconsistency or race conditions.
* A mutex provides two fundamental operations
	* Locking
	* Unlocking
* If the lock is available process takes ownership of he lock and proceeds with its critical section of code where it accesses the shared resource.
* Once the thread completes its critical section, it releases the mutex by unlocking it. this allow other waiting thread to acquire the shared resources.
* The concept of mutual exclusion ensures that only one thread can execute the critical section.