---
creation date: 2023-06-07 13:28
modification date: Wednesday 7th June 2023 13:28:26
tag: #linux #network
---

#### Source:
[LJ](https://linuxjourney.com/lesson/rsync)
[DO](https://www.digitalocean.com/community/tutorials/how-to-use-rsync-to-sync-local-and-remote-directories)

--------------------------------------

#### Explanation about it:

* `rsync` also used to copy a data from different hosts.
* rsync stands for `short for remote synchronizations`
* it is very similar to rsync.
* rsync have a special algorithm that checks in advanced if there is already data that you are copying to and will copy over the differences.
* some rsync options
	* v - verbose
	* r - recursive into directories
	* h - human readable output
	* z - compressed for easier transfer, great for slow connections

```
#copy files on the same host
rsync -zvr /local/directory/one /local/directory/two
```

```
#copy files from local to remote host

rsync /local/directory root@address:/remote/directory
```

```
#copy files from remore host to local host

rsync root@address:/remote/directory /local/directory
```

