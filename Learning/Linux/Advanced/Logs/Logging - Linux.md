---
creation date: 2023-06-06 15:58
modification date: Tuesday 6th June 2023 15:58:13
tag: #OS #Linux #Log
---

#### Source:
[LJ](https://linuxjourney.com/lesson/system-logging)

-----------------------------------------------------
#### What is it?

* Services, kernel, daemons, etc on your system are constantly doing something, this data is actually sent to be saved on your system in the form of logs.
* This allows us to have a human readable journal of the events that are happening on our system.
* This data is usually kept in the /var directory.

-----------------------------------------------------
#### Why we need it?

* **Troubleshooting and Debugging:** 
	* Logs provide a valuable information for diagnosing and resolving issues in a linux system.
* It monitor security related things like failed login attempts and unauthorized access attempts.
* logs helps to monitor and analyze system performance.

-----------------------------------------------------
#### Where it comes?

* Linux journal and process events notes.
-----------------------------------------------------
#### Explanation about it:

* syslog is used to sends information to the system logger.
* syslog actually contains many components, one of the important ones is daemon running called syslogd(newer linux distributions use rsyslogd).
* Each application can have their own logging rules and generate different log files.

```
less /var/log/syslog
```

#### [[Syslog]]

-----------------------------------------------------
#### Benefit:


-----------------------------------------------------
#### Simple Explanation:


-----------------------------------------------------
#### Visual image of topic:


-----------------------------------------------------

#### Links: