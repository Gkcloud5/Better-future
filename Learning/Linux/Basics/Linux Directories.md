#### Source:
[JTP](https://www.javatpoint.com/linux-directories)
[TP](https://www.tutorialspoint.com/unix/unix-directories.htm)


* A directory is a file, it is used to store a file name and the related information.
* Linux uses a hierarchical structure for organizing files and directories.
	* This structure is often referred to as a directory tree.
	* the tree has a single root node, the '/' and all other directories are contained below it.


#### Home Directory:

* The directory in which you find yourself when you login is called your home directory

```
#go home directory
cd ~

#Go any other user's home directory
cd ~username

#To go last directory
cd -
```


#### Absolute and relative path names:

* Elements of a path name separated by a '/'.
* **Absolute** Path name always begin with a '/'.

```
/etc/passwd
/users/kumar
```

* **Relative:** A pathname can also be relative to your current working directory.
* relative pathnames never begin with /.

```
chem/notes
gok/users
```
