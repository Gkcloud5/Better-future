#### Source:
[LJ](https://linuxjourney.com/lesson/filesystem-hierarchy)

* Filesystems can vary with how they are structured.
* But for the most part they should conform to the filesystem hierarchy standard.

* /  --> root directory of the entire filesystem hierarchy, everything is nestled under this directory.
* /bin --> Ready to run programs, most basic command such as ls, cp
* /boot --> Contains kernel boot loader files.
* /dev --> Device files.
* /etc -->  Core system configuration directory, should hold only configuration files and not any binaries.
* /home --> Personal directories for users, holds your documents
* /lib --> Holds library files, it has precompiled code.
* /media --> used as an attachment point for removable media like USB drives
* /mnt --> Temporarily mounted filesystem
* /opt --> Optional application software packages
* /