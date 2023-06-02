#### Source:
[LJ](https://linuxjourney.com/lesson/dev-directory)


#### 1. /dev directory:

* When you connect a device to your machine, it generally needs a device driver to function properly.
* You can interact with device drivers through device files or device nodes.
* these files are just like regular files, you can use program such as ls, cat, etc to interact with them.
* these device files are generally stored in the `/dev` directory.

```
ls /dev
```


#### 2. Device types:

```
ls -l /dev

brw-rw----   1 root disk      8,   0 Dec 20 20:13 sda
  
crw-rw-rw-   1 root root      1,   3 Dec 20 20:13 null
  
srw-rw-rw-   1 root root           0 Dec 20 20:13 log
  
prw-r--r--   1 root root           0 Dec 20 20:13 fdata
```