#Advanced 

#### Source: 
[Regular expression](https://www.learnpython.org/en/Regular_Expressions)
[youtube](https://www.youtube.com/watch?v=y9XCjDJ0Rgc)


**Matching pattern in text. in python.**

##### Package
```
import re
```


##### Example1:
```
import re
str = "Gk is hope guy"
result = re.compile("is")
ans = result.search(str)
print(ans)
```
![[Pasted image 20230415124538.png]]

.  --> this matches any character except a newline.
^ --> Matches the start of the string.
$ --> Matches the end of the string or just before the new line.
[syntax](https://docs.python.org/3/library/re.html#regular-expression-syntax%22RE%20syntax)

