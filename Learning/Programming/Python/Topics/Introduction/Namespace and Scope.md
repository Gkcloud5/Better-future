
#### Source: [Namespace and scope](https://www.programiz.com/python-programming/namespace)
[Namespace-2](https://insideaiml.com/blog/Namespaces-and-Scope-in-Python-1142)

**Variables are pointers, they are pointing objects, Namespace is a dictionary, in dictionary variable name is key and object is value.**

* Built-in variable
* Global variable 
* Local variable

![[Pasted image 20230309233304.png]]


Each module creates it's own **Global namespace**

A **Local namespace** is created when a function is called.

### Scope:
 There are various unique namespaces defined, we may not able to access all of them from every part of the program. the concept of scope comes into play.

 A scope is the portion of a program from where a namespace can be accessed directly without any prefix.

 **3 Nested scope:**
	 * Scope of the current function which has local names
	 * Scope of the module which has global names
	 * Outermost scope which has built-in names

 ```
 # global_var is in the global namespace
global_var = 10

def outer_function():
    #  outer_var is in the local namespace 
    outer_var = 20

    def inner_function():
        #  inner_var is in the nested local namespace 
        inner_var = 30

        print(inner_var)

    print(outer_var)

    inner_function()

# print the value of the global variable
print(global_var)

# call the outer function and print local and nested local variables
outer_function()

```

![[Pasted image 20230319194812.png]]

#### Example with built-in keyword:

```
# define global variable 
global_var = 10

def my_function():
    # define local variable
    local_var = 20

    # modify global variable value 
    global global_var
    global_var = 30

# print global variable value
print(global_var)

# call the function and modify the global variable
my_function()

# print the modified value of the global variable
print(global_var)
```

![[Pasted image 20230319195006.png]]

