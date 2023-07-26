---
creation date: 2023-06-12 20:51
modification date: Monday 12th June 2023 20:51:55
tag: 
---

#### Source:
[LJ](https://linuxjourney.com/lesson/dhclient)

--------------------------------------

#### Explanation about it:

* DHclient starts up on boot and gets a list of network interfaces from the dhclient.conf file.
* For each interface listed it tries to configure the interface using the DHCP protocol.

```
dhclient
```

