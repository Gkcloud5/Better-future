#### Source:
[YT](https://www.youtube.com/watch?v=Z68js3PxzW0&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=89)

#### Problem is:

* Let consider 5 philosophers in round table, p0 to p4.
* Rice is center of table
* each philosopher have a plate
* Totally 5 fork is there c0 to c4.

![[Pasted image 20230516212348.png]]

* Each philosopher will do 2 activity
	* Eat
	* Think
* in order to eat  philosopher need 2 fork
* Let consider p0 is eating
	* So p1 and p4 not possible to eat
	* p2 or p3 have a chance to eat
* If each philosopher is hunger and each one have 1 fork then [[Deadlock]] will occur.

#### Solution for this issue:

##### We are using semaphore to solve this issue:

* we will use wait and signal operation

![[Pasted image 20230516213132.png]]

##### Code:

```
// declare five semaphores
semaphore fork[5];

// define a function for the philosopher
void philosopher(int i) {
  // acquire the left fork
  wait(&fork[i]);

  // acquire the right fork
  wait(&fork[(i + 1) % 5]);

  // eat
  // ...

  // release the left fork
  signal(&fork[i]);

  // release the right fork
  signal(&fork[(i + 1) % 5]);
}

```