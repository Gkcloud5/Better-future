#### Source:
[YT](https://www.youtube.com/watch?v=ntFKeKUQiQo&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=36)
[GFG](https://www.geeksforgeeks.org/readers-writers-problem-set-1-introduction-and-readers-preference-solution/)


#### About problem:

* A file shared between reader and writer process.
* reader can read a content of file
* Writers process can perform read and write operations
* Some of the process only want to read the resources and some of the processes are writers, which want to write

#### Constraints:

* Allow multiple readers to read the file simultaneously.
* When a reader process accessing the file then write process is not allowed to access file.
* When write process accessing the file then no other process is allowed to access a file.

##### Semaphore solution:

```
// declare two semaphores
semaphore reading = 1;
semaphore writing = 1;

// define a function for the reader
void reader() {
  // acquire the reading semaphore
  wait(&reading);

  // read from the resource
  // ...

  // release the reading semaphore
  signal(&reading);
}

// define a function for the writer
void writer() {
  // acquire the writing semaphore
  wait(&writing);

  // write to the resource
  // ...

  // release the writing semaphore
  signal(&writing);
}

```

![[Pasted image 20230516200332.png]]

