---
creation date: 2023-06-07 23:26
modification date: Wednesday 7th June 2023 23:26:00
tag: 
---

#### Source:
[LJ](https://linuxjourney.com/lesson/subnet-math)

--------------------------------------

#### Explanation about it:

* Subnet masks important to figure out how many hosts we can have on our subnet.
* IP address 192.168.1.0
* subnet mask 255.255.255.0

```
192.168.1.165  = 11000000.10101000.00000001.10100101
255.255.255.0  = 11111111.11111111.11111111.00000000
```

* If it's in 1 then it is masked, so only possible hosts are from the 00000000 region.
* we need to subtract 2 host, because we need to assign broadcast address and subnet address so possible host count is 254.
* 192.168.1.1 to 192.168.254
