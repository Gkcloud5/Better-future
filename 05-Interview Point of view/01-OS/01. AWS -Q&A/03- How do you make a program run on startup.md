
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


##### 3. Using *init.d*:
* File location `/etc/init.d`

```
#!/bin/sh
case "$1" in
	start)
		sudo sh /etc/reboot_message.sh
		;;
	*)
		;;
esac
exit 0
```