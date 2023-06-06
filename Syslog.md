---
creation date: 2023-06-06 21:33
modification date: Tuesday 6th June 2023 21:33:55
tag: 
---

#### Source:
[LJ](https://linuxjourney.com/lesson/syslog)

--------------------------------------

#### Explanation about it:

* Syslog service manages and sends logs to the system logger.
* Rsyslog is an advanced version of syslog.
* output of the all the logs the syslog service collects can be found at /var/log/syslog

```
less /etc/rsyslog.d/50-default.conf
```

```
# First some standard log files.  Log by facility.
#
auth,authpriv.*                 /var/log/auth.log
*.*;auth,authpriv.none          -/var/log/syslog
#cron.*                         /var/log/cron.log
#daemon.*                       -/var/log/daemon.log
kern.*                          -/var/log/kern.log
#lpr.*                          -/var/log/lpr.log
mail.*                          -/var/log/mail.log
#user.*                         -/var/log/user.log

```

* rules to log files are denoted by t