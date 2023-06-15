---
creation date: 2023-06-15 16:56
modification date: Thursday 15th June 2023 16:56:03
tag: 
---

#### Source:
[LJ](https://linuxjourney.com/lesson/etc-hosts)

--------------------------------------

#### Explanation about it:

* Before our machine actually hits DNS to do a query, it first looks locally on our machine

##### /etc/hosts:

* It contains mapping of some hostnames to IP address.

```
root@root:~# cat /etc/hosts
127.0.0.1 localhost
127.0.1.1 root

# The following lines are desirable for IPv6 capable hosts
::1     ip6-localhost ip6-loopback
fe00::0 ip6-localnet
ff00::0 ip6-mcastprefix
ff02::1 ip6-allnodes
ff02::2 ip6-allrouters

```

##### /etc/resolv.conf

* It used to map DNS nameservers

```
root@root:~# cat /etc/hosts.allow

nameserver 127.0.0.53
options edns0 trust-ad
search .
```

