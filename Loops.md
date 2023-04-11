#Basics #Loops 

Two types of loop:
	* For Loop
	* While Loop

#### For loop:
* For loop iterate over a given sequence
```
list = [1, 5, 7, 8]
for prime in list:
    print(prime)
```

##### range in for loop:
```
for x in range(5):
    print(x)
```


#### While loop:
* while loop repeat as long as a certain boolean condition is met.
```
count = 0
while count < 5:
    print(count)
    count +=1
```

#### break and continue statement:

`Break` statement is used to exit a for loop or while loop, whereas `continue` is used to skip the current block, and return to the `for` or `while` statement.
```
count =0
while True:
      print(count)
      count +=1
      if count >= 5:
        break

for x in range(10):
    if x % 2 == 0:
       continue
    print(x)
```

![[Pasted image 20230411225545.png]]

#### Else in for loop:

* While statement failed then else part executed
* If a break statement executed inside a loop the Else part is skipped.
* Else part is executed even if there is a continue statement.

```
count = 0
while(count<5):
     print(count)
     count+=1
else:
    print("last count value is %d" % (count))

for i in range(1, 10):
    if(i%5==0):
        break
    print(i)
else:
    print("this is not printed because for loop is terminated because of break but not due to fail in condition")

```

![[Pasted image 20230411230023.png]]

