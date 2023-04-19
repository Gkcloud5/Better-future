#Pattern #logical #Python 

#### Source:
[youtube](https://www.youtube.com/watch?v=KcejV_MaUdg&list=PLIFRUdRwOM0_2VMQ_8BBY4SIEXNjkwfW5&index=3)

#### Need to print:
```
*
**
***
****
***
**
*
```

#### Program:
```
rows = int(input("Enter a number"))
for i in range(0,rows):
   for j in range(0, i+1):
       print("* ", end = "")
   print()

for i in range(rows, 0, -1):
    for j in range(0, i-1):
       print("* ", end = "")
    print()
```

##### Program logic information:
* Here we divided two parts 
	* One is `i` increment
	* Second one is `i` decrement part
* All other logic is same as like previous pattern program

