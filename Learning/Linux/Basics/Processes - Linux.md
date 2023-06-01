#### Source:
[TP](https://www.tutorialspoint.com/unix/unix-processes.htm)

* When we execute a program on linux system, the system creates a special environment for that program. this environment contains everything needed for the system to run the program as if no other program were running on the system.
* OS tracks process through process id `pid`

#### Starting a process:

* Two ways to run a process
	* foreground processes
	* background process

##### Foreground processes:

* every process that you start runs in the foreground. it gets input from the keyboard and sends its output to the screen.