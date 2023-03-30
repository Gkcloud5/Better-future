#### Source: [Lambda](https://www.programiz.com/python-programming/anonymous-function)

**A lambda function is a special type of function without the function name.**

`lambda : print('Hello World')`


#### Lambda function declaration:

We use `lambda` keyword instead of `def` to create a lambda function.
`lambda argument(s) : expression`

![[Pasted image 20230330201709.png]]

##### Example 1:
```
greet = lambda : print ('Hello World')

greet()

#output
Hello world
```


##### lambda function with an argument:

```
# lambda that accepts one argument
greet_user = lambda name : print('Hey there,', name)

# lambda call
greet_user('Delilah')

# Output: Hey there, Delilah
```



