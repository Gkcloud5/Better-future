
#### Source:
[HR](https://www.hackerrank.com/challenges/swap-case/problem?isFullScreen=true)

#### Question:
![[Pasted image 20230602164931.png]]

#### Solution -1:(Using special method)

```
def swap_case(s):
    return s.swapcase()

if __name__ == '__main__':
    s = input()
    result = swap_case(s)
    print(result)
```