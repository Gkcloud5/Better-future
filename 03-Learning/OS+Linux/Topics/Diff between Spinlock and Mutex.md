**Process synchronization** --> **Critical Section Problem**

#### Source:
[YT](https://www.youtube.com/watch?v=XKBjwQQJ0qk&list=PL3uLubnzL2Tlbyrr2GFVRE7Azo8FJe-dJ&index=9)


#### Differences:

* Both are used to avoid critical section problem by using lock method
	* But mutex is **sleeping** lock
		* We are not using while loop here
	* Spinlock is a **busy lock**
		* Because it continually check if critical section is available or not
* Mutex requires [[Context switching]]
