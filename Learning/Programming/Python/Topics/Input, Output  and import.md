## About Input, Output and import:

#### Source: [I&O](https://www.programiz.com/python-programming/input-output-import)

### Python output:
* `print` function to print output.

```
print('Python is powerful')
# Output: Python is powerful
```

##### Syntax of print();
`print(object= separator= end= file= flush=)`

* **Object** --> Values to be printed
* **sep(optional)** --> it separate objects inside a print function
* **end(optional)** --> It add specific values like `\n` and ` ` 
* **file(optional)** --> `print file.tx` 
* **flush(optional)** --> Boolean output specifying if the output is flushed or buffered
```
python
print("Hello, World!", flush=True)

#output

```

##### 1. Print statement:
```
print('Good Morning!')
print('It is rainy today')
```

![[Pasted image 20230307223454.png]]

##### 2.Print() with end parameter:
```
# print with end whitespace
print('Good Morning!', end= ' ')

print('It is rainy today')
```
![[Pasted image 20230307223554.png]]

##### 3. Print() with sep parameter:
```
print('New Year', 2023, 'See you soon!', sep= '. ')
```
![[Pasted image 20230307223646.png]]
* Here output separated by comma.


#### Output formatting:

 * We can format a output by using `str.format()` function.

##### Example 1:
```
x = 5
y = 10

print('The value of x is {} and y is {}'.format(x,y))
```

**Output**
```
The value of x is 5 and y is 10
```

*Here curly{} are used as a placeholders, we can specify the order by using tuple index*

##### Example 2:

```
x = 5
y = 10
xy = ('19', '39', '7')

print('The value of x is {} and y is {}'.format(x,y))
print('here xy(0) is {} and 1 is {}'.format(xy[0],xy[1]))
```

**Output**
```
The value of x is 5 and y is 10
here xy(0) is 19 and 1 is 39
```


### Python input:

 Input taken from users, for this we will use `input()` function.

```
input(prompt)
```

##### Example 1:
```
# using input() to take user input
num = input('Enter a number: ')

print('You Entered:', num)

print('Data type of num:', type(num))
```

![[Pasted image 20230307224929.png]]

