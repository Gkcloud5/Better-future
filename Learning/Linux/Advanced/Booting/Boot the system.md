#### Source:
[LJ](https://linuxjourney.com/lesson/boot-process-overview)

* Linux boot process can be broken down in 4 simple stages:
	* BIOS
	* Bootloader
	* Kernel
	* Init

#### [[BIOS]]:

* BIOS --> Basic input and output system
* It initialize the hardware and makes sure with a Power-on-self test(POST) that all the hardware is good to go.
* The main job of the BIOS is to load up the bootloader

#### [[Bootloader - linux]]:

* Bootloader loads the kernel into memory and then starts the kernel with a set of kernel parameters.
* One of the most common bootloader is GRUB.

#### [[Kernel]]:

* When the kernel is loaded, it immediately initialize device and memory.
* Main job of the kernel is to load up the init process.

#### init:

* Remember the init process is the first process that gets started
* init starts and stops essential service to the system
* 
