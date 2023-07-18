### About:

* It will check given string in another string and return index value if it's matched

```
str1="gokul testing find string function"
str2="find"
print(str1.find(str2))
```

![[Pasted image 20230718223857.png]]

* Passing initial value and final value
	* will check particular portion in string
	* It's optional one

```
str1="gokul testing find string function"
str2="find"
print(str1.find(str2,10,20))
print(str1.find(str2,16,20))
```

![[Pasted image 20230718224022.png]]

* If value not matching then it will return `-1`
