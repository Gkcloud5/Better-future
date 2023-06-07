---
creation date: 2023-06-07 14:43
modification date: Wednesday 7th June 2023 14:44:07
tag: #linux #OS #network
---

#### Source:
[LJ](https://linuxjourney.com/lesson/nfs-network-file-share)

--------------------------------------

#### Explanation about it:

* Most standard network file share for linux is NFS.
	* Network file system.
* NFS allows a server to share directories and files with one or more clients over the network.

```
#setting up nfs client

service nfsclient start
mount server:/directory /mount_directory
```
