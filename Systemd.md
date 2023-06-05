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
* systemd does not
