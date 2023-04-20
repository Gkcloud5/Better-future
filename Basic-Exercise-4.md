#### Exercise:
**Remove first `n` characters from a string**
  Write a program to remove characters from  a string from zero up to n and return a new string

#### Sample output:

![[Pasted image 20230420175533.png]]

#### Logic Think:
* Get a word from user
* Get a index number from user to remove a letters in string
* Need to remove a letter from index 0 to number that user give

#### Program:

```
def remove_chars(str,num):
    str = str[0: 0:] + str[num::]
    print(str)
    
remove_chars("pynative", 4)
remove_chars("pynative", 2)

```

#### Output:

![[Pasted image 20230420181139.png]]
