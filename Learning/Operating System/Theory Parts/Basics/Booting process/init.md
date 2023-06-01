#### Source:
[wiki](https://en.wikipedia.org/wiki/Init#:~:text=In%20Unix%2Dbased%20computer%20operating,the%20system%20is%20shut%20down.)
[init](https://www.javatpoint.com/linux-init)


* **init** is the first process started during booting of the OS.
* **init** is a daemon process that continues running until the system is shutdown.
* it is automatically adopts all orphaned processes.
* It reads the script stored in the file `/etc/inittab`. and it take care of everything that a system do system initialization like setting the clock, initializing the serial port and so on.
* It determine how the system should be set up in each run level and sets default run level.
* After determining the default runlevel of the system, init starts all background processes required to run the system.


#### Runlevels:

* It is a software configuration of linux system which permits only a selected group of processes to exit.

![[Pasted image 20230429135341.png]]

