---
creation date: 2023-06-05 20:24
modification date: Monday 5th June 2023 20:30:03
tag: #kernel #OS #init
---

#### Source:
[LJ](https://linuxjourney.com/lesson/upstart-overview)

--------------------------------------

#### Explanation about it:

* It was developed by canonical, so it was the init implementation on ubuntu while
* Modern ubuntu installation systemd is now used.
* to find our init is upstart or not

```
/usr/share/upstart
```

* To start a jobs

```
start on runlevel [235]
stop on runlevel [0]
```

* It means that it will start setting up networking on runlevel 2,3 or 5 and will stop networking on runlevel 0.
* Upstart working ways
	* First, it loads up the job configurations from /etc/init
	* once a startup event occurs, it will run jobs triggered by that event.
	* These jobs will make new events and then those events will trigger more jobs.
	* Upstart continues to do this until it completes all the necessary jobs.

#### Operations:

```
#to check status
initctl status networking

#start
initctl start networking

#stop
initctl stop networking

#restart
initctl restart networking
```

