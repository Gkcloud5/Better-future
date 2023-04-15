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

