---
creation date: 2023-06-06 21:44
modification date: Tuesday 6th June 2023 21:44:09
tag: 
---

#### Source:
[LJ](https://linuxjourney.com/lesson/kernel-logging)

--------------------------------------

#### Explanation about it:

##### /var/log/dmesg:

* On boot-time your system logs information about the kernel ring buffer.
* This shows us information about hardware drivers, kernel information and status during bootup and more.
* this log reset on every boot.
* dmesg is the best place to look issue regarding hardware.

##### /var/log/kern.log:

* This is another log to view kernel information.
* this logs the information and events on your system