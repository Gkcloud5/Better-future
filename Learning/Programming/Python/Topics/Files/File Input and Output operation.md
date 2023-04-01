#### Source: [IO operation](https://www.programiz.com/python-programming/file-operation)

* A file is generally storage of data.

**File operation takes place in the following order:
	* Open a file
	* Read or write
	* close the file**

##### Open a file:

 We use `open()` method to open files.

```
file1 = open("test.txt")
```

##### To give option:

```
file1 = open("test.txt", "r")
```

![[Pasted image 20230401151521.png]]


#### Reading files in python:

 we use `read()` method to read it's content.

```
file1 = open("test.txt", "r")

read_content = file1.read()
print(read_content)
```

![[Pasted image 20230401151839.png]]

#### Closing files in python:

 After performing operations on the file we need to properly close the file

we need to use `close()` to close a file.

```
file1 = open("test.txt", "r")

read_content = file1.read()
print(read_content)

file1.close()
```

![[Pasted image 20230401152217.png]]