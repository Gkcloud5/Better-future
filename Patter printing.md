#Pattern #logical

#### Source:
[Youtube](https://www.youtube.com/watch?v=x8IXcg7m57s)

#### Need to print:
```
*
**
***
****
*****
```

##### Logics think:
* First step, need to consider row and column
	* In above example there is a 5 row and totally 5 columns

#### Solution:
```
rows = int(input("enter the row value"))

for i in range(1, rows+1):
    for j in range(1, i+1)
        print("*", end=" ")
    print()
```


![[Pasted image 20230419173538.png]]

##### Program logic information:

```
rows = int(input("enter the row value"))
```
* Above line help to get a value to determine how many rows need to print

```
for i in range(1, rows+1):
```
* Value need to start from 1 and final value should tot