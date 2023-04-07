## About Data type:


#### Source: [Data Type](https://www.programiz.com/python-programming/variables-datatypes)

* How can we store a data in code that's data type

## Python Data Types

![[Pasted image 20230223185225.png]]

#### Numeric data type:
*It used to hold a numeric values*
* Int
* Float
* complex

**We can use `type()` function to know which class a variable or a value belongs to

```
num1 = 5
print(num1, 'is of type', type(num1))

num2 = 2.0
print(num2, 'is of type', type(num2))

num3 = 1+2j
print(num3, 'is of type', type(num3))
```

![[Pasted image 20230225233106.png]]

#### List Data type:

List is an ordered collection of similar or different types of items separated by commas and enclosed within brackets `[]`.

```
languages = ["Swift", "Java", "Python"]
```

*Here we created a list with a name of **languages** with 3 string values inside it*

##### Access List items:

We need to use index numbers to access list data type values

```
languages = ["Swift", "Java", "Python"]

# access element at index 0
print(languages[0])   # Swift

# access element at index 2
print(languages[2])   # Python
```


#### Tuple data type:

**Tuple is same as list but it's a immutable, tuples once created cannot be modified**

*We use parentheses `()` to store items of tuple*

```
product = ('Xbox', 499.99)
```

* Here product is tuple with a string value and integer value

##### Access Tuple items:

We need to use index number to access tuple items in python.

```
# create a tuple 
product = ('Microsoft', 'Xbox', 499.99)

# access element at index 0
print(product[0])   # Microsoft

# access element at index 1
print(product[1])   # Xbox
```


#### String data type:

* String is a sequence of characters represented by a either single or double quotes.

```
name = 'Python'
print(name)  

message = 'Python for beginners'
print(message)
```

![[Pasted image 20230225234229.png]]

#### Set Data type:

* Set is an unordered collections of unique items. set is defined by values separated by commas inside brackets `{}`.

```
# create a set named student_id
student_id = {112, 114, 116, 118, 115}

# display student_id elements
print(student_id)

# display type of student_id
print(type(student_id))
```

![[Pasted image 20230225234947.png]]


#### Dictionary Data types:

* Python dictionary is an ordered collection of items. It stores elements in key and value pairs
* Here keys are unique identifiers that are associated with each value.

```
# create a dictionary named capital_city
capital_city = {'Nepal': 'Kathmandu', 'Italy': 'Rome', 'England': 'London'}

print(capital_city)
```

![[Pasted image 20230225235911.png]]

