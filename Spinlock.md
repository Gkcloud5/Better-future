**Process synchronization** --> **Critical section **

#### Source:
[YT](https://www.youtube.com/watch?v=XKBjwQQJ0qk&list=PL3uLubnzL2Tlbyrr2GFVRE7Azo8FJe-dJ&index=9)

#### What is spinlock:

* This lock which causes a thread/process trying to acquire it to simply wait in a loop ("spin") while repeatedly checking if the lock is available.
	* This protects the critical section from being accessed concurrently.

![[Pasted image 20230529185502.png]]

* Since the thread remains active but is not performing a useful task, the use of such a lock is a kind of busy waiting.(Busy for waiting)
* 