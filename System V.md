---
creation date: 2023-06-05 20:16
modification date: Monday 5th June 2023 20:16:55
tag: #kernel #init
---

#### Source:

[LJ](https://linuxjourney.com/lesson/sysv-overview)

--------------------------------------------

#### Explanation about it:

* You can find which init implemented in OS by running following command

```
/etc/inittab
```

* System V starts and stops processes sequentially.
* it have different run levels are set from 0 to 6.
	* 0: Shutdown
	* 1: Single user mode
	* 2: Multiuser mode without networking
	* 3: Multiuser mode with networking
	* 4: Unused
	* 5: Multiuser mode with networking and GUI
	* 6: Reboot

#### Services:

```
service --status-all

#start
service networking start

#stop
service networking stop

#restart
service networking restart
```
