#### Exercise:
**Initialize dictionary with default values**


#### Sample output:

![[Pasted image 20230423141353.png]]


#### Logic think:

* In dictionary we have `fromkeys()` method to accomplish this thing

#### Program:

```
employees = ['Kelly', 'Emma']
defaults = {"designation": 'Developer', "salary": 8000}
thisdict = dict.fromkeys(employees, defaults)


print(thisdict)
```

#### Output:

![[Pasted image 20230423141606.png]]