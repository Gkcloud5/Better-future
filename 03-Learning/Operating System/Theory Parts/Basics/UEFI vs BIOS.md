#### Source:
[GFG](https://www.geeksforgeeks.org/uefiunified-extensible-firmware-interface-and-how-is-it-different-from-bios/)


* **Unifies Extensible Interface**

#### Limitation of BIOS:

* BIOS can boot drives of less then 2TB.
* BIOS runs in 16-bit processor mode has only 1MB of space to execute
* It can't initialize multiple hardware devices at once, thus leading a slow booting process

#### About UEFI:

* It is a type of firmware interface used in modern computers to replace the traditional BIOS.
* UEFI provides a more advanced and flexible interface than BIOS.
* One of the main diff between BIOS and UEFI is the way they handle system initialization.
* UEFI is stored in non-volatile memory on the motherboard and is capable of directly loading the OS from the hard drive.
* UEFI is installed at the time of manufacturing and is the first program that runs when booing the computer.

#### Booting process of a UEFI:

* UEFI does not look for a MBR in first sector
* UEFI behaves like a miniaturized OS that sits between firmware and the OS.
* The OS boots directly in UEFI.
* UEFI stores initialization data in an EFI file partition in non-volatile memory, rather than in the firmware.
* During the POST procedure, UEFI firmware scans all of the bootable storage devices that are connected to the system for a valid GPT(Guided Partition Table).
* The firmware itself scans the GPT to find an EFI System partition to boot from.