#### Source:
[YT](https://www.youtube.com/watch?v=x1tg2YUCs-c&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=15)


#### About single thread:

* By default every process will contains only one thread
* This thread defines flow of execution through the process code, with its own program counter.

![[Pasted image 20230519203314.png]]

**Code:** It is useful to store instruction of process.
**Data:** Useful to store global variable
**Files:** Used to store opened file information regarding process
**Registers:** It contains registers, program counter.
**Stack:** it is a local variable.

#### Problem in single traded process:

* Assume single thread is blocked so CPU need to wait for execution till the thread unblocked.
* 