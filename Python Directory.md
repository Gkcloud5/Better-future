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
