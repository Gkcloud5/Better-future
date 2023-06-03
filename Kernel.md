#### Source:
[LJ](https://linuxjourney.com/lesson/boot-process-kernel)

#### initrd vs initramfs

* Kernel manages our system hardware, however not all drivers are available to the  kernel during bootup.
* so we depend on temporary file system, it contains all the basic module to boot up a kernel.
* 