#### Source:
[YT](https://www.youtube.com/watch?v=yw__NPExEH4&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=35)

#### About Bounded buffer problem:

* It is also known as producer and consumer problem.
* It involves two types of concurrent processes
	* Producers
	* Consumers
		* Who share a fixed-size buffer or queue
* The goal of bounded buffer problem is to ensure that producers and consumers can safely access the buffer without encountering issues.

#### Challenges in the bounded buffer:

##### Mutual Exclusion:
* Only one process should access the buffer at a given time to avoid concurrent access conflicts.

##### Full Buffer Detection:
* Producers should not overwrite data in the buffer when it is full. 
* They need to wait until space becomes available.

##### Empty Buffer Detection:
* Consumers should not consume data from empty buffer.
* They need to wait until data is available for consumption

##### Bounded waiting:
* Processes should not wait indefinitely.
* There should be a mechanism to limit the waiting time and ensure progress.

#### Example:

```
// declare two semaphores
semaphore empty = 1;
semaphore full = 0;

// define a function for the producer
void producer() {
  // acquire the empty semaphore
  wait(&empty);

  // put data in the buffer
  // ...

  // release the full semaphore
  signal(&full);
}

// define a function for the consumer
void consumer() {
  // acquire the full semaphore
  wait(&full);

  // take data out of the buffer
  // ...

  // release the empty semaphore
  signal(&empty);
}

```