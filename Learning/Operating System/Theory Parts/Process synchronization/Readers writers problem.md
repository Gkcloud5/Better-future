#### Source:
[YT](https://www.youtube.com/watch?v=ntFKeKUQiQo&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=36)

#### About problem:

* A file shared between reader and writer process.
* reader can read a content of file
* Writers process can perform read and write operations
* Some of the process only want to read the resources and some of the processes are writers, which want to write

#### Constraints:

* Allow multiple readers to read the file simultaneously.
* When a reader process accessing the file then write process is not allowed to access file.
* When write process accessing the file then no other process is allowed to access a file.