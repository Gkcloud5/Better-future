#### Source:
[YT](https://www.youtube.com/watch?v=boSYXHtW03M&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=34)

#### About Swap instruction:

* It is a machine instruction and atomic instruction.
* The swap instruction operates on two memory locations, typically referred to as 
	* Variables
	* Registers

#### Sample Example:

```c++
// declare a global variable to represent the lock
bool lock = false;

// define a function to acquire the lock
void acquire_lock() {
  //atomically swap the value of the lock variable with true
  bool old_value = swap(&lock, true);

  // if the lock was not already acquired, then enter the critical section
  if (old_value == false) {
    // critical section
  }
}

// define a function to release the lock
void release_lock() {
  // set the lock variable to false
  lock = false;
}

```


#### YT example:

![[Pasted image 20230516181028.png]]

