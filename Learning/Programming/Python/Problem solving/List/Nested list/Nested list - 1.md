#### Source:
[HR](https://www.hackerrank.com/challenges/nested-list/problem?isFullScreen=true)


#### Question:

![[Pasted image 20230530210047.png]]

#### Sample output:

![[Pasted image 20230530210111.png]]


#### Solution 1: (By using for loop and if condition)

```python
student_list = []
if __name__ == '__main__':
    for _ in range(int(input())):
        name = input()
        score = float(input())
        student_list.append([name,score])
        
student_list.sort(key = lambda x: x[1])

second_mark = student_list[1][1]
second_grade = []
print(student_list)
for x in student_list:
    if second_mark == x[1]:
        second_grade.append(x)
        
second_grade.sort(key = lambda x: x[0])
for x in range(0, len(second_grade)):
    print (second_grade[x][0])
```


#### Solution 2: (By using calling function)

```

```