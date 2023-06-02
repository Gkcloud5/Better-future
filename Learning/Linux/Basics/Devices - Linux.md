#### Source:
[LJ](https://linuxjourney.com/lesson/dev-directory)


#### 1. /dev directory:

* When you connect a device to your machine, it generally needs a device driver to function properly.
* You can interact with device drivers through device files or device nodes.
* these files are just like regular files, you can use program such as ls, cat, etc to interact with them.
* these device files are generally stored in the `/dev` directory.

```
ls /dev
```


#### 2. Device types:

```
ls -l /dev

brw-rw----   1 root disk      8,   0 Dec 20 20:13 sda 
crw-rw-rw-   1 root root      1,   3 Dec 20 20:13 null 
srw-rw-rw-   1 root root           0 Dec 20 20:13 log 
prw-r--r--   1 root root           0 Dec 20 20:13 fdata
```

* Columns are as follows from left to right
	* Permission
	* owner
	* group
	* Major device number
	* Minor device number
	* timestamp
	* device name
* In command you can see type of file in each line
	* c - character
	* b - block
	* p - pipe
	* s - socket


#### Character Device:

* These devices transfer a data but one character at a time.
* you will see lot of pseudo devices(/dev/null) as character devices.
	* These devices are not really physically connected to the machine, but they allow the OS greater functionality.

#### Block device:

* These devices transfer data, but in large fixed-size blocks.
* Harddrives and filesystem

#### Pipe Devices:

* Pipe allow two or more processes to communicate with each other.

#### Socket:

* It used to communicate with many process at once.


#### 3. Device Names:

* ##### SCSI devices:
	* Small Computer System Interface.
	* It is a protocol used to allow communication between disks, printers, scanners and other peripherals to your system.
	* Common SCSI device
		* /dev/sda - First hard disk
		* /dev/sdb - Second hard disk

* ##### Pseudo Devices:
	* /dev/zero -- accepts and discard all the input
	* /dev/null -- accepts and discards all input, produces no output.


### [sysfs](https://linuxjourney.com/lesson/sysfs)


#### udev:

* udev systems dynamically creates and remove device files for us dependin