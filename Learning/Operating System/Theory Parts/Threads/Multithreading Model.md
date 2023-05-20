#### Source:
[GFG](https://www.geeksforgeeks.org/multi-threading-models-in-process-management/)

#### About multithreading model:

* Multi threading-it is a process of multiple threads executes at same time.
* Many OS supports kernel thread and user thread in a combined way, example of such system is Solaris.

#### 3-Types of model:

##### Many-to-one model:

![[Pasted image 20230520134959.png]]

* Here many no.of user thread mapped to single kernel thread.
* Here we have only one kernel thread then multiptocess architecture is not possible.

##### One-to-one model

 ![[Pasted image 20230520135311.png]]

* It mainly implemented to solve a issue from many to one mode, it solve parallelism, concurrency.
* Here Each user thread mapped to each kernel thread.
* So if one thread is blocked then is no issue, other thread will take care of a process

##### Many-to-many:

 ![[Pasted image 20230520135723.png]]

* 