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
* While a program is running in the foreground and is time-consuming, no other commands can be run because the prompt would not be available until the program finishes processing and comes out.

##### Background processes:

* Background processes runs without being connected to your keyboard.
* advantage of background process is that you can run other commands
	* No need to wait for complete one process
* simplest way to start a background process, need to add & at the end of the command.

```
ls ch*.doc &
```


#### Listing running processes:

* `ps` command

```
ps

ps -f
```

![[Pasted image 20230601085420.png]]


#### Stopping processes:

* signal --> `CTRL+C`
* get process id and kill it

```
ps -f

kill process_id
```


#### Parent and child process:

* Each linux process has two ID numbers
	* pid
	* ppid ==> Parent process ID.

#### Zombie and orphan processes:

* Parent process is killed before kill child process so child process will not have a parent so this process called a orphan processes.
* z state --> zombie state
	* This process is dead and not being used