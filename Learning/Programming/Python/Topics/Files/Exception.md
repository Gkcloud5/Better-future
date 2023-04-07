#### Source: [Exception](https://www.programiz.com/python-programming/exceptions)

**An Exception is an unexpected event that occurs during program execution.**
```
divide= 7 / 0
```
The above code causes an exception as it is not possible to divide a number by 0.

#### Logical Errors(Exceptions):

* Errors that occur at runtime are called exceptions or logical errors.

Some errors:
	* Try to open a file that does not exist `FileNotFuondError`
	*  Try to divide a number by zero `ZerodivisionError`


![[Pasted image 20230407141451.png]]


#### Built-in Exceptions:
```
print(dir(locals()['__builtins__']))
```

