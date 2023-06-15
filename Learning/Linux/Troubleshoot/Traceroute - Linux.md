---
creation date: 2023-06-15 13:42
modification date: Thursday 15th June 2023 13:42:18
tag: 
---

#### Source:
[LJ](https://linuxjourney.com/lesson/traceroute)

--------------------------------------

#### Explanation about it:

* Traceroute command is used to see how packets are getting routed.
* It works by sending packets with increasing TTL values, starting with 1, so the first router gets the packet and it decrements the value by one
	* The router sends back an ICMP time exceeded message back to us.
* And then next packet gets a TTL of 2, so it makes it past the first router.

```
root@root:~# traceroute google.com
traceroute to google.com (172.217.13.174), 64 hops max
  1   38.102.86.65  0.363ms  0.196ms  0.194ms
  2   96.45.197.101  1.122ms  0.975ms  0.789ms
  3   199.167.153.53  0.431ms  0.334ms  0.507ms
  4   199.167.154.218  1.237ms  0.794ms  0.942ms
  5   199.167.154.221  0.748ms  0.572ms  0.690ms
  6   207.66.123.107  0.578ms  0.538ms  0.522ms
  7   72.15.48.50  0.872ms  0.851ms  0.750ms
  8   66.207.192.242  0.597ms  0.465ms  0.485ms
  9   108.170.251.17  1.833ms  1.587ms  1.591ms
 10   108.170.231.63  1.932ms  1.329ms  1.599ms
 11   172.217.13.174  0.690ms  0.698ms  0.737ms

```

