#### Source:
[LJ](https://linuxjourney.com/lesson/boot-process-bios)


#### BIOS:

* First step in the linux boot process is the BIOS which performs system integrity checks.
* we can use BIOS firmware to change the boot order of your harddisks.
* Check system time and mac address, etc,...
* BIOS main goal is to find the system bootloader.
* Once the BIOS boots up the hard drive, it searches for the boot block to figure out how to boot up the system.
* Depending on partition
	* It will look MBR or GPT
		* MBR is located in the first sector of the hard drive, first 512 bytes.
		* MBR contains the code to load another program somewhere on the disk. this program in turn actually loads up bootloader.


#### UEFI:

* There is another way to boot up your system instead of using BIOS.
* Unified extensible firmware interface.
* Most hardware out there today comes with UEFI firmware.
* first sector of a GPT disk is reserved for a "protective MBR" to make it possible to boot BIOS based machine.
* UEFI stores all the information about startup in an `.efi` file.
* File is stored on a special partition called EFI system partition on the hardware.
* inside this partition it will contain the bootloader.

