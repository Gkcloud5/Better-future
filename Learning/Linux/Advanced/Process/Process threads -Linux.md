---
creation date: 2023-06-05 22:26
modification date: Monday 5th June 2023 22:28:02
tag: #kernel #process 
---

#### Source:
[LJ](https://linuxjourney.com/lesson/process-threads)

-----------------------------------------------------
#### What is it?

* A thread is a basic unit of execution within a process.
* thread sharing the same memory space and resource with their parent process so sometimes we call it as lightweight process.
* Threads helps to running a multiple tasks simultaneously or in parallel.
-----------------------------------------------------
#### Why we need it?

* **To improve performance:**
	* threads can run concurrently on the multiple CPU's, which significantly improve the performance of an application
* It improve resource utilization.
-----------------------------------------------------
#### Where it comes?

* Process synchronization
* multiprogramming OS

-----------------------------------------------------
#### Explanation about it:

* Threads are used to execute the same program.
* They are often referred to as lightweight processes.
* If a process has one thread it is single-threaded and if a process has more than one thread it is multi-threaded.
* Each thread represents an independent sequence instructions.
* OS scheduler determines the order and duration of execution for each thread.
* Threads within a process share the same memory space and resources, allowing them to communicate and coordinate easily.
* When the OS starts executing a program, it typically creates a primary thread, known as the main thread. the main thread is responsible for initiating the execution of other threads.
-----------------------------------------------------
#### Benefit:

* **Concurrency:** threads enable concurrent execution of multiple tasks within a single process. this concurrency allows for better utilization of system resource.
* **Responsiveness**
* **Resource efficiency:** Threads share the same memory space and resources of the parent process.

-----------------------------------------------------
#### Simple Explanation:

* Threads operation is same like process, trying to do a run a program, but here threads is created inside a process, creation of thread is completely depends on a process, if process needs multiple thread then it may create it
* Created thread share a same memory space of a parent process so it does not need that instruction should be in main memory. 
* Here no need for context switching, simply OS scheduler will change the thread and execute a process.
* 
-----------------------------------------------------
#### Visual image of topic:


-----------------------------------------------------

#### Links:
* [[Threads]]
* [[Threads in OS]]