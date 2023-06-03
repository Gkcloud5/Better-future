#### Source:
[LJ](https://linuxjourney.com/lesson/boot-process-kernel)

#### initrd vs initramfs

* Kernel manages our system hardware, however not all drivers are available to the  kernel during bootup.
* so we depend on temporary file system, it contains all the basic module to boot up a kernel.
* in older version of linux, this job given to the initrd(initial ram disk).
	* kernel would mount the initrd. get the necessary boot drives.
* This days we have something called the initramfs, this is temporary root filesystem that is built itself to load all the necessary drivers for the real root filesystem.

#### Mounting the root filesystem:

* Now kernel has all the modules it needs to create a root device and mount the root partition.
* first root partition is actually mounted in read only mode so that fsck run safely and check for system integrity.
	* Afterwards it remounts the root filesystem.
* Then the kernel locate the init program and execute it