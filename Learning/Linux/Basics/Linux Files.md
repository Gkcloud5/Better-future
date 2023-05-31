#### Source:
[TP](https://www.tutorialspoint.com/unix/unix-file-management.htm)
[JTP](https://www.javatpoint.com/linux-files)

* All data in linux is organized into files.
* All files are organized into directories.
* These directories are organized into a tree-like structure called the filesystem.

#### Basic types of file:

* **Ordinary Files**
	* It contains data, text or program instructions.
* **Directories:**
	* It store both special and ordinary files.
* **Special Files:**
	* Some special files provide access to hardware such as hard drives, CD-ROM drive,  modems and ethernet adaptors.


#### Listing files:

* List the files and directories stored in current directory

```
ls

#to get more information
ls -l

```

![[Pasted image 20230531225551.png]]


#### Metacharacters:

* Metacharacters have a special meaning in linux.
	* * use to match 0 or more characters
	* ? use to match with single character

```
#example
ls ch*.doc

#output
ch01-1.doc   ch010.doc  ch02.doc    ch03-2.doc 
ch04-1.doc   ch040.doc  ch05.doc    ch06-2.doc
ch01-2.doc ch02-1.doc c
```


#### Hidden files:

* An invisible file is one, the first character of which is the `dot(.)` 

```
ls -a
```


#### Creating Files:
