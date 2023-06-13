---
creation date: 2023-06-12 20:49
modification date: Monday 12th June 2023 20:49:09
tag: 
---

#### Source:
[LJ](https://linuxjourney.com/lesson/route)

--------------------------------------

#### Explanation about it:

* we can see routing table by using `route` command.

```
#Add route
route add -net IPaddress/23 gw GATEWAYADDR

#Delete a route
route del -net IPADDRESS/23

#Add route
ip route add IPADDress/23 via GATEWAYADDRESS

#Delete route
ip route delete IPaddress/23 via GatewayAddress
```