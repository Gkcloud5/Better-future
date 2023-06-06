
#### Source:
[HR](https://www.hackerrank.com/challenges/find-a-string/problem?isFullScreen=true)


#### Sum:

![[Pasted image 20230606210932.png]]

#### Solution 1:(Chat gpt)

```
def count_substring(string, sub_string):
    count = 0
    start = 0

    while True:
        index = string.find(sub_string, start)
        if index == -1:
            break
        count += 1
        start = index + 1

    return count

if __name__ == '__main__':
    string = input().strip()
    sub_string = input().strip()
    
    count = count_substring(string, sub_string)
    print(count)
```

