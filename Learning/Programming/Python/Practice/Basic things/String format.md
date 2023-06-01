#string #Basics  #Python 

#### Source: [String format](https://www.learnpython.org/en/String_Formatting)

**Print a variable inside print double quote function**

```
# This prints out "Hello, John!"
name = "Gk"
print("Hello, %s!" % name)

```

![[Pasted image 20230409200227.png]]

##### Use string and number:

```
str1="GK"
num1=26
print("%s is %d year old" % (str1, num1))
```

#### Some basic argument specifiers:

%s -- String (Or any object with string representation)
%d -- Integers
%f  -- Floating point numbers

##### Test1:
You will need to write a format string which prints out the data using the following syntax: `Hello John Doe. Your current balance is $53.44.`

```
data = ("John", "Doe", 53.44)
format_string = "Hello %s %s. Your current balance is $%s."

print(format_string % data)
```