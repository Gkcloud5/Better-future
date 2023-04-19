#Pattern #logical #Python 

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
    for j in range(1, i+1):
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
* Value need to start from 1 and final value should row+1
* This line will decide how many rows we need to print
* let consider value range(1, 6) then totally 5 rows will be created

```
for j in range(1, i+1):
```
* This line about column information
* Here we depends on `i` value. 
* `i+1` reason is here we need to print two * on 2nd row and three * in 3rd row so it depends on i value so that only we consider i here
```
print("*", end=" ")
```
* `end=" "` is used to separate a output from space instead of new line

