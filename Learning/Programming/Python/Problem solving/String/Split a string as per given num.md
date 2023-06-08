#### Source:
[HR](https://www.hackerrank.com/challenges/text-wrap/problem?isFullScreen=true)

#### Question:

![[Pasted image 20230608232003.png]]


#### Solution 1: own - Using for and if condition:

```
import textwrap


def wrap(string, max_width):
    letter = 0
    string_split = ""
    for i in string:
        letter = letter + 1
        string_split += i
        #print (len(string_split), string_split, i, letter)
        if len(string_split) == max_width:
            print (string_split)
            #return string_split
            string_split = ""
        if letter == len(string):
            return string_split
            #print ("last word", string_split)
    
if __name__ == '__main__':
    string, max_width = input(), int(input())
    result = wrap(string, max_width)
    print(result)
```

#### Solution 2: using chatGPT
