#### Exercise:
**Print characters from a string that are present at an even index number**
 Write a program to accept a string from the user and display characters that are present at an even index number

#### Sample output:

![[Pasted image 20230420160944.png]]

#### Logic Think:
* Get a string input
* Identify a even index
* print a character that's in even index

#### Program:

```
str = input("Enter a string")
str_len = len(str)

for i in range(0, str_len):
    if(i%2  == 0):
        print(str[i])
```


#### Output:

![[Pasted image 20230420175246.png]]

