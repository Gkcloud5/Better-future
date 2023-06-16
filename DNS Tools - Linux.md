---
creation date: 2023-06-16 14:39
modification date: Friday 16th June 2023 14:39:29
---

**Tags:** #DNS #linux 

#### Source:
[LJ](https://linuxjourney.com/lesson/dns-tools)

--------------------------------------

#### Explanation about it:

##### nslookup:

* name server lookup tool is used to query name servers to find information about resource records.

```
nslookup google.com

Server:         127.0.0.53
Address:        127.0.0.53#53

Non-authoritative answer:
Name:   google.com
Address: 172.217.13.174
Name:   google.com
Address: 2607:f8b0:4020:805::200e

```

##### dig:

* Domain information groper

```

root@root:~# dig google.com

; <<>> DiG 9.18.12-0ubuntu0.22.04.1-Ubuntu <<>> google.com
;; global options: +cmd
;; Got answer:
;; ->>HEADER<<- opcode: QUERY, status: NOERROR, id: 14729
;; flags: qr rd ra; QUERY: 1, ANSWER: 1, AUTHORITY: 0, ADDITIONAL: 1

;; OPT PSEUDOSECTION:
; EDNS: version: 0, flags:; udp: 65494
;; QUESTION SECTION:
;google.com.                    IN      A

;; ANSWER SECTION:
google.com.             44      IN      A       172.217.13.174

;; Query time: 4 msec
;; SERVER: 127.0.0.53#53(127.0.0.53) (UDP)
;; WHEN: Fri Jun 16 09:16:18 UTC 2023
;; MSG SIZE  rcvd: 55

```

