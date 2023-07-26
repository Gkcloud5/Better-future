#### Source:
[Yt](https://www.youtube.com/watch?v=q7yksMlPlJU&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=33)

#### What is test and set instruction:

* It is a synchronization mechanism
* It uses a test and set instruction to provide the synchronization among the processes executing concurrently.

#### About it:

* **Atomic instruction:** All the instruction in procedure will execute one life cycle.

![[Pasted image 20230516173621.png]]

* Test and set is a machine instruction.
	* Machine instruction means form 0 and 1,

![[Pasted image 20230516174555.png]]

* **test and set:** test the instruction and making a value true to run a process in critical section


#### Spin lock instruction:

``` c++
bool lock = false;  // Shared lock variable

// Acquiring the lock
while (test_and_set(&lock) == true) {
    // The lock is already acquired, so the current thread spins and waits
}

// Critical section: Only one thread can access the shared resource at a time

// Releasing the lock
lock = false;
```



#### Example to resolve mutual exclusion, progress and bounded waiting:

``` c++
bool lock = false;  // Shared lock variable

int maxAttempts = 100;  // Maximum number of attempts to acquire the lock

// Component A
for (int attempt = 0; attempt < maxAttempts; attempt++) {
    while (test_and_set(&lock) == true) {
        // The lock is already acquired, so Component A spins and waits
    }
    
    // Critical section: Only Component A can access the shared resource at a time

    // Release the lock
    lock = false;
}

// Component B
for (int attempt = 0; attempt < maxAttempts; attempt++) {
    while (test_and_set(&lock) == true) {
        // The lock is already acquired, so Component B spins and waits
    }
    
    // Critical section: Only Component B can access the shared resource at a time

    // Release the lock
    lock = false;
}

```