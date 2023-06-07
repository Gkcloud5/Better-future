---
creation date: 2023-06-07 13:23
modification date: Wednesday 7th June 2023 13:23:33
tag: #linux #network
---

#### Source:
[LJ](https://linuxjourney.com/lesson/network-file-sharing)

--------------------------------------

#### Explanation about it:

* Simple file sharing tool in `scp` command.
* scp stands for secure copy.
* It allows us to copy from one host over to another host on the same network.
* It works via ssh

```
#copy file from local to remote

scp myfile.txt root@Ipaddress:/remote/directory
```

```
#Copy file from remote to local

scp root@Address:/remote/directory/file.txt /local/directory
```

```
#Copy directory from local to remote

scp -r mydir root@address:/remote/directory
```
