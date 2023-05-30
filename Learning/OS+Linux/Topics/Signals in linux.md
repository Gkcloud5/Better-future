**Process synchronization** --> **Interprocess Communication**

#### Source:
[YT](https://www.youtube.com/watch?v=p-qltZWQKAs&list=PL3uLubnzL2Tlbyrr2GFVRE7Azo8FJe-dJ&index=10)

* In OS, signals are a form of inter-process communication that allows processes or threads to send notifications to each other.
* They are used to handle various events or exceptional conditions that occur during program execution.
* Signals are used to inform a process about events such as the termination of another process, user interrupt, hardware exceptions, or  specific conditions like segmentation fault.
	* When a signal is sent to a process, the OS interrupts the normal flow of  execution and delivers the signal to the target process.
* list of signals `kill -l`
* A signal in linux is a notification sent to a process to indicate that an important event has occurred.
* Signal can be sent by the kernel, by other processes or by the process itself.


##### Actions:

* When a process receives a signal, it can take one of several actions
	* Ignore the signal
	* Handle the signal by calling a signal handler function
	* Terminate

3u