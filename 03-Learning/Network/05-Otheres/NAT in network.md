---
creation date: 2023-08-02 11:18
modification date: Wednesday 2nd August 2023 11:18:08
---

**Tags:** #network 

#### Source:
[NAT](https://www.geeksforgeeks.org/network-address-translation-nat/)

--------------------------------------

### Explanation about it:

* Generally, inorder to access a internet one public IP address is needed, but we can use private IP address in our private network
* idea of NAT is allow multiple devices to access the internet through a single public address.

### 2. NAT working:
 * Border router is configured as NAT.
 * Router which has one interface in local network and one interface in the global.
 * When packet traverse outside the local network, NAT converts local IP address to a global IP address.
 * When packet enters the local network, the global IP address is converted to local IP address.

![[Pasted image 20230802113045.png]]

