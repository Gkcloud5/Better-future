#### Source:
[BB](https://www.javatpoint.com/boot-block-and-bad-block-in-operating-system)


#### About Boot Block:

* It is a region of hard disk, floppy disk that contains machine code to be loaded into RAM by a computer system's built-in-firmware
* When a computer starts running or reboot, it needs an initial program to run. this initial program is known as the bootstrap program.
* It must initialize all aspects of the system
	* First initialize the CPU registers, device controllers, main memory and then starts the OS
	* Bootstrap program finds the OS kernel on disk to do its job and then loads that kernel into memory.
	* Last jumps to the initial address to begin the OS execution.

![[Pasted image 20230429143251.png]]
