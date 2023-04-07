#### Source: [Directory](https://www.programiz.com/python-programming/directory)

A directory is a collection of files and subdirectories. A directory inside a directory is known as a subdirectory.
Python has the `os` module that provides us with many useful methods to work with directories.


#### Get Current directory:
We can get the present working directory using the `getcwd` method of the `os` module.

##### Example:
```
import os
print(os.getcwd)
```

#### Changing directory in python:
```
chdir()
```
The new path that we want to change into must be supplied as a string to this method. And we can use both the forward-slash or the backward-slash to separate the path elements

```
import os
os.chdir('C:\\Python33')

print(os.getcwd())

output: C:\Python33
```


#### List directories and files in python:
```
listdir()
```
This method takes in a path and returns a list of subdirectories and files in that path

```
import os
print(os.getcwd())
C://Python33

os.listdir()
['dir1',
'dir2',
'file.txt']

os.listdir('G:\\')
['dir2',
'dir3',
'file1.txt']
```

#### Making a new directory:
```
mkdir()
```

```
os.mkdir('test')

os.listdir()
['test']
```

#### Renaming a directory:
```
rename()
```

It needs two arguments
	First argument      --> old name
	Second argument --> Second name

```
import os
os.listdir()
['test']

#rename
os.rename('test', 'new_name')

os.listdir()
['new_name']
```