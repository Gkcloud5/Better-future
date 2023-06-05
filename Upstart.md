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

* It means that it will start