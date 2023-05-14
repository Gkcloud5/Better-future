[YT](https://www.youtube.com/watch?v=AOrmV3NcBKU&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=14)

#### About Remote Procedure call:

* Calling procedure which located in remote machine.

#### How it implemented?

* Client calls client stub(program) or client proxy.
* Client stub packs parameters into a message, this process called marshaling.
* Client OS sends message to server using a system call
* Server calls s