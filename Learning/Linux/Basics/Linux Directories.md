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

```
#To know current working directory
pwd
```


#### Listing Directory:

```
#List a directory
ls dirname
ls /usr/local
```

#### Creating Directories:

```
mkdir name_of_directory
mkdir gokul

#create directory inside another directory
mkdir /tmp/test

#create multiple directory
mkdir gok1 gok2
```

#### Creating parent directories:

* create a new directory at that same time create another directory from newly created directory

```
mkdir -p /gok/user/dir1
```

-p --> it creates all the necessary directories for you.


#### Removing directories:

```
#rem
```

