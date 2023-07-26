#### Source:
[LJ](https://linuxjourney.com/lesson/boot-process-init)

* It is a first process get started and it starts all the other essential services on our system.

#### Three major implementation of init in Linux:

##### System V init(sysv):

* This is traditional init system.
* it sequentially starts and stops processes based on startup scripts.
* state of the machine is denoted by runlevels, each runlevel starts or stops a machine in a different way.

##### Upstart:

* This is the init you will find on older ubuntu installation.

##### Systemd:

* This is new standard for init.
* it is goal oriented.
* Basically you have a goal that you want to achieve and systemd tries to satisfy the goal's dependencies to complete the goal.
