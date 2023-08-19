
### Source:

[BD](https://www.baeldung.com/linux/run-script-on-startup)

**Running scripts on startup is a common practice in linux and other operating systems to automate various tasks and ensure that certain processes are initiated whenever system boots up.**

##### Some purposes:
* ###### Server services:
	* Start automatically some server application
		* Web server
		* Database server
		* Application server
* ###### Running Backup scripts
* ###### To do automated tasks:
	* Done system updates
	* log cleanup

### Ways to run a program on startup:

##### Created a script:
```
#reboot_message.sh

#!/bin/bash
echo "Last reboot time: $(date)" > /etc/motd

#Giving permission
chmod +x reboot_message.sh
```

##### 1. Using *Cron*:

```
crontab -e

@reboot sh /etc/reboot_message.sh
```

* @reboot --> It will execute our code once at startup

##### 2. Using *rc.local*:
* File location is `/etc/rc.d/rc.local`
* add a following line in above file

```
sh /etc/reboot_message.sh

###Chekcing permission
chmod +x /etc/rc.d/rc.local
```

##### 3. Using *systemd*:
* File location `/etc/systemd/system`

```
[Unit]
Description=Reboot message systemd service

[Service]
Type=simple
ExecStart=/bin/bash /etc/reboot_message.sh

[Install]
WantedBy=multi-user.target

```

* Unit     ==> Contains genera metadata, like human-readable description
* Service ==> Describes the process and demonizing behavior, along with the command to start the service
* Install   ==> Enables the service to run at startup using the folder specified in *WantedBy* to handle dependencies.

```
#Set Permission
chmod 644 /etc/systemd/system/reboot_message.service
systemctl enable reboot_message.service
```