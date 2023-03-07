## About **Type conversion**

#### Source: [Type conversion](https://www.programiz.com/python-programming/type-conversion-and-casting)

**It is the process of converting data from one type to another type.

#### 2 types of conversion:
* Implicit conversion
* Explicit conversion

##### Implicit conversion:
 In some situations, python automatically convert data type, *Python always convert smaller data types to larger data types to avoid data loss*

**Example:**
```
integer_number = 123
float_number = 1.23

new_number = integer_number + float_number

# display new value and resulting data type
print("Value:",new_number)
print("Data Type:",type(new_number))
```

![[Pasted image 20230307203534.png]]

In above example, `int` is a lower data type when compare to `float` that is a reason for showing output in float data type.

**Type Error:** generally, we get type error while doing this type of data conversion. for avoiding it we will use another type(*Explicit conversion*) of data conversion.

##### Explicit Type Conversion:
 Here user will convert a data type from one type to required data type, we use built