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

* we can use `vi` editor to create directory files.

```
vi filename
```

* This will open file with given name. now press `i` to come into the edit mode.

```
This is linux file. I created it for the first time
```

* Save a file
	* press `esc` to come out of the edit mode


#### Display content of a file:

* we can use `cat` command to see the content of a file.

```
cat filename

#to show line number
cat -b filename
```


#### Counting words:

* we can use wc command to get a count of the total number of lines

```
wc filename
2  19 103 filename
```

![[Pasted image 20230531231406.png]]

```
#To get muiltiple files information
wc filename1 filename2 filename3
```


#### Copying Files:

```
cp source_file destination_file
```

#### Renaming file:

```
mv olf_file new_file
```

#### Deleting files:

```
rm filename
```


#### [Rename](https://www.javatpoint.com/linux-rename-v)


