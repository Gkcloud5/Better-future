#Basics #variable
## About Variable:

#### Source: [Variables](https://www.programiz.com/python-programming/variables-constants-literals)

* Purpose of *variable* is to store a value. 
	* a = 10.
	* Here `a` is identifier

**In programing, a variable is a container to hold a data

			`number = 10`
*Here number storing the value 10*


#### Assigning values to variables:

```
# assign value to site_name variable
site_name = 'programiz.pro'

print(site_name)

# Output: programiz.pro

```

![[Pasted image 20230223181543.png]]


#### Assigning multiple values to multiple variables:

```
a, b, c = 5, 3.2, 'Hello'

print(a)  # prints 5
print(b)  # prints 3.2
print(c)  # prints Hello 
```

*Assign same value = to multiple variables*
```
site1 = site2  = 'programiz.com'

print(site1)  # prints programiz.com
print(site2)  # prints programiz.com
```


#### Rules for Naming variables:

* Variable names should have a combination of letters in lowercase (**a to z**) or uppercase (**A to Z**) or digits (**0 to 9**) or an underscore `(__)`
```
snake_case
MACRO_CASE
camelCase
CapWords
```

* Create a name that makes sense. For example, `vowel` makes more sense than `v`.
* If you want to create a variable name having two words, use underscore to separate them
```
my_name
current_salary
```
* Python is case-sensitive. So **num** and **Num** are different variables
*  Avoid using [keywords](https://www.programiz.com/python-programming/keywords-identifier) like if, True, class, etc. as variable names.

#### Python constants:

* A constant is a special type of variable whose value cannot be changed
* In Python, constants are usually declared and assigned in a [module](https://www.programiz.com/python-programming/modules)
*Create a **constant.py**:*
```
# declare constants 
PI = 3.14
GRAVITY = 9.8
```

*Create a **main.py**:*
```
# import constant file we created above
import constant

print(constant.PI) # prints 3.14
print(constant.GRAVITY) # prints 9.8
```

In the above example, we created the **constant.py** module file. Then, we assigned the `constant` value to `PI` and `GRAVITY`.
After that, we create the **main.py** file and import the `constant` module. Finally, we printed the constant value.

#### Python Literals:

**Literals are representations of fixed values in a program, they can be numbers, characters or strings, etc

*Literals are often used to assign values to variables or constants*

##### Numeric literals:
**Numeric Literals are immutable (unchangeable). Numeric literals can belong to 3 different numerical types: `Integer`, `Float`, and `Complex`.**

![[Pasted image 20230223183527.png]]


##### Boolean Literals:
* There are two Boolean literals: `true` and `false`
		`pass = true`

##### Literal Collections:
* List
* Tuple
* Dictionary
* Set

**Examples:**
```
# list literal
fruits = ["apple", "mango", "orange"] 
print(fruits)

# tuple literal
numbers = (1, 2, 3) 
print(numbers)

# dictionary literal
alphabets = {'a':'apple', 'b':'ball', 'c':'cat'} 
print(alphabets)

# set literal
vowels = {'a', 'e', 'i' , 'o', 'u'} 
print(vowels)
```

![[Pasted image 20230223184152.png]]
