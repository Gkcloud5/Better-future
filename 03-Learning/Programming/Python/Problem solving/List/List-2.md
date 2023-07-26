#### Source:
[HR](https://www.hackerrank.com/challenges/finding-the-percentage/problem?isFullScreen=true)

#### Question:

![[Pasted image 20230531120508.png]]


#### Sample Output:

![[Pasted image 20230531120538.png]]


#### Output:

```
if __name__ == '__main__':
    n = int(input())
    student_marks = {}
    for _ in range(n):
        name, *line = input().split()
        scores = list(map(float, line))
        student_marks[name] = scores
    query_name = input()

def find_average_marks(student_marks, query_name):
     marks = student_marks[query_name]
     total_marks = sum(marks)
     number_of_marks = len(marks)
     average_marks = total_marks / number_of_marks
     return round(average_marks, 2)
     
average_marks = find_average_marks(student_marks, query_name)
print(f"{average_marks:.2f}")
```

#### Things i learnt:

* Create function and passing arguments and get result is **Best practice**
* **round**
* How to print float value ==> print(f"{average_marks:.2f}")