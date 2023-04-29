#### Source:
[wiki](https://en.wikipedia.org/wiki/Init#:~:text=In%20Unix%2Dbased%20computer%20operating,the%20system%20is%20shut%20down.)


* init is the first process started during booting of the OS.
* init is a daemon process that continues running until the system is shutdown.
* it is automatically adopts all orphaned processes.
* It reads the script stored in the file `/etc/inittab`. and it take care of everything that a system do s