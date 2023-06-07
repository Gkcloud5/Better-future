#### Question:

![[Pasted image 20230607225615.png]]

![[Pasted image 20230607225630.png]]

#### Solution1: (For and if loop)

```
if __name__ == '__main__':
    s = input()
    

def any_char(string):
    for i in string:
        if i.isalpha() == 1 or i.isdigit() == 1:
            return True
            break
    return False
        
def any_alpha(string):
    for i in string:
        if i.isalpha():
           return True
           break
    return False
       
def any_digit(string):
    for i in string:
        if i.isdigit():
            return True
            break
    return False

def any_lower(string):
    for i in string:
        if i.islower():
            return True
            break
    return False

def any_upper(string):
    for i in string:
        if i.isupper():
            return True
            break
    return False

print (any_char(s))
print (any_alpha(s))    
print (any_digit(s))
print (any_lower(s))
print (any_upper(s))
```

#### Solution 2:

```
string = "Hello123"

print(any(c.isalnum() for c in string))
print(any(c.isalpha() for c in string))
print(any(c.isdigit() for c in string))
print(any(c.islower() for c in string))
print(any(c.isupper() for c in string))
```
