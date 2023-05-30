#### Source:
[HR](https://www.hackerrank.com/challenges/nested-list/problem?isFullScreen=true)


#### Question:

![[Pasted image 20230530210047.png]]

#### Sample output:

![[Pasted image 20230530210111.png]]

#### Sample Input:

![[Pasted image 20230530215928.png]]

#### Solution 1: (By using for loop and if condition)

```python
student_list = []
if __name__ == '__main__':
    for _ in range(int(input())):
        name = input()
        score = float(input())
        student_list.append([name,score])
        
student_list.sort(key = lambda x: x[1])


unique_mark = list(set(map(lambda x: x[1], student_list)))
unique_mark.sort()


print(len(unique_mark))
second_mark = 0

#Get second mark 
if len(unique_mark) < 3:
    if unique_mark < 0:
        second_mark = unique_mark[1]
    else
        second_mark = min(unique_mark)
else:
    second_mark = unique_mark[1]

print(second_mark)


second_grade = []

for x in student_list:
    if second_mark == x[1]:
        second_grade.append(x)
        
second_grade.sort(key = lambda x: x[0])
for x in range(0, len(second_grade)):
    print (second_grade[x][0])
    
    
```


#### Solution 2: (Chat GPT solution)

```python
students = []
if __name__ == '__main__':
    for _ in range(int(input())):
        name = input()
        score = float(input())
        students.append([name, score])

# Find the second lowest grade
grades = set([student[1] for student in students])
second_lowest_grade = sorted(grades)[1]


# Get the names of students with the second lowest grade
students_with_second_lowest_grade = [student[0] for student in students if student[1] == second_lowest_grade]


students_with_second_lowest_grade = sorted(students_with_second_lowest_grade)


# Print the names of students with the second lowest grade
for student_name in students_with_second_lowest_grade:
    print(student_name)
```

