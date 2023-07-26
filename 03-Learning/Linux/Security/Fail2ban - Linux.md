---
creation date: 2023-06-17 16:02
modification date: Saturday 17th June 2023 16:02:19
---

**Tags:** #linux #fail2ban #security

#### Source:
[YT](https://www.youtube.com/watch?v=9cHspiqCdsM&list=PLTnRtjQN5ieb3ljl02823yOnUax7sF1DD&index=8)

--------------------------------------

#### Explanation about it:

* One of the security feature for linux.
* It will save server from brute force attack

##### What is brute force attack?

* It is targeting authentication protocol.
	* Send random username and password to login server
	* Attackers mostly target most privilege account.

#### All about fail2ban:

* It ban IP based on logs
* In logs we have information about failed authentication.

```
#install
apt install fail2ban -y 

#status
systemctl status fail2ban 
```

```
#Configugration for SSH

Location to edit file -->  /etc/fail2ban/jail.local

[DEFAULT]

#Override /etc/fail2ban/jail.d/00-firewalld.conf:
banaction = iptables-multiport

[sshd]
enabled = true
port = 28
filter = sshd
logpath = /var/log/auth.log
maxretry = 3
bantime = 3600
```

```
Check fail2ban ssh jail status --> sudo service fail2ban status

Check particular service status --> fail2ban-client status sshd

restart fail2ban --> service fail2ban restart

Unban ip --> fail2ban-client set sshd unbanip 46.31.24.24
```