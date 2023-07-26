---
creation date: 2023-06-05 20:37
modification date: Monday 5th June 2023 20:37:51
tag: #kernl #OS #init
---

#### Source:
[LJ](https://linuxjourney.com/lesson/systemd-overview)

--------------------------------------

#### Explanation about it:

* It is emerging standard for init.
* Systemd uses goals to get your system up and running. Basically you have a target that you want to achieve 
	* This target also has dependencies that we need to achieve.
* Systemd is extremally flexible and robust. it does not follow strict sequence to get processes started.
* Here's what happens during typical systemd boot:
	* First, systemd loads its configuration files, usually located in /etc/systemd/system or /usr/lib/systemd/system.
	* Then it determines its boot goal, which is usually default.target
	* Systemd figures out the dependencies of the boot target and activates them.
* systemd does not just start and stop services, it can mount filesystems, monitor your network sockets, etc and because of that robustness it has different types of units it operates.
	* Service.units - these are the services we have been starting and stopping, these unit files end in .service
	* Mount units - These mount filesystems, these unit files and in .mount.
	* Target units - these group together other units, the files end in .target.

```
[Unit]  
Description=My Foobar
Before=bar.target

[Service]  
ExecStart=/usr/bin/foobar

[Install]
WantedBy=multi-user.target
```


#### Some commands:

```
systemctl list-units

#status
systemctl status networking.service

#start
systemctl start networking.service

#stop
systemctl stop networking.service

#restart
systemctl restart networking.service

```
