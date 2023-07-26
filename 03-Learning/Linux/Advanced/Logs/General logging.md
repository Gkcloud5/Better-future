---
creation date: 2023-06-06 21:40
modification date: Tuesday 6th June 2023 21:40:15
tag: 
---

#### Source:
[LJ](https://linuxjourney.com/lesson/general-logging)

--------------------------------------

#### Explanation about it:

* you can see many log files in our system.
* there are two general log files
	* /var/log/messages
	* /var/log/syslog

##### /var/log/messages:

* This log contains all non-critical and non-debug messages, includes message logged during bootup, auth, cron, daemon, etc,

##### /var/log/syslog:

* This logs everything except auth messages, it's exremely useful for debugging errors on your machine.
