#### Source:
[YT](https://www.youtube.com/watch?v=8wcuLCvMmF8&list=PL3uLubnzL2Tlbyrr2GFVRE7Azo8FJe-dJ)

#### 1. It comes under:

##### 1.1 Process synchronization:

* Process synchronization in OS refers to the coordination and control mechanisms employed to manage the execution order and access to shared resources among multiple concurrent processes.
* The need for process synchronization arises when multiple processes or threads access shared resources simultaneously.
* Process synchronization in OS is like the traffic control system that ensures smooth and safe interaction between processes.

##### 1.2 Approach:

* Hardware Approach
* Software Approach
	* Semaphore
	* Mutex

#### 2. Semaphore vs Mutex:

* We need to avoid clashes between process.
* By using semaphore and mutex we are going to do allocate and release a resource without any collision.
* Basic difference between both is the way the operation is done
	* Semaphore is a signaling approach
	* Mutex is a lock based approach


##### 2.1 Semaphore:

* It is all about wait() and signal(). this will indicate if the process is acquiring a resource or releasing a resource.
* It is a integer
	* Binary
	* Counting
* Multiple program threads can access a finite instance of resources.
* 
##### 2.2 Mutex:

*  It is all about locking.
* Here the process shall acquire lock on the mutex object if the resource has to be acquired
* It is an object
* Mutex allow multiple program threads to access a single resource, but, with a restriction of not accessing simultaneously.
* 