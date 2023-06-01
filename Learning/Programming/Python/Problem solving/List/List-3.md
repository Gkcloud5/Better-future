
#### Source:
[HR](https://www.hackerrank.com/challenges/python-lists/problem)

#### Question and sample output:

![[Pasted image 20230601164007.png]]

![[Pasted image 20230601164021.png]]


#### ChatGPT solution:

```
if __name__ == '__main__':
    N = int(input())
    my_list = [] 
    for _ in range(N):
        command = input()
        
        #insert
        if command.startswith("insert"):
            _, index, value =  command.split()
            index = int(index)
            value = int(value)
            my_list.insert(index,value)
        elif command.startswith("print"):
            print (my_list)
        elif command.startswith("remove"):
            _, value = command.split()
            value = int(value)
            my_list.remove(value)
        elif command.startswith("append"):
            _, value = command.split()
            value = int(value)
            my_list.append(value)
        elif command.startswith("sort"):
            my_list.sort()
        elif command.startswith("pop"):
            my_list.pop()
        elif command.startswith("reverse"):
            my_list.reverse()
```


#### Things i learnt:

``` 
for _ in range(N):
```
* By using above command we can get input from user as per integer value we provide

```
command.startswith("insert")
```
* By using above command we can easily match condition as per first element

```
_, index, value =  command.split()
```
* Here, i am split a given content and store those split content to variable.