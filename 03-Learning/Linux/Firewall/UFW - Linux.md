---
creation date: 2023-06-17 14:55
modification date: Saturday 17th June 2023 14:55:35
---

**Tags:** #linux #firewall #ufw

#### Source:
[YT](https://www.youtube.com/watch?v=lt2itMlreQo&list=PLTnRtjQN5ieb3ljl02823yOnUax7sF1DD&index=5)

--------------------------------------

#### Explanation about it:

* UFW stands for Uncomplicated firewall

**do not enable ufw before setup firewall rule because it can actually lock you out**


```
#check status
ufw status

#diable
ufw diable

#deny
ufw default deny incoming

#allow
ufw default allow incoming

#disble service
systemctl stop ufw

#delete rule
ufw status numbered
ufw delete *number*
```

* stop service and add rule is best practice

