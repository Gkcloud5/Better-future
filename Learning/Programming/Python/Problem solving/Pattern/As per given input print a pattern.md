
#### Source:
[HR](https://www.hackerrank.com/challenges/designer-door-mat?isFullScreen=true)

#### Question:

![[Pasted image 20230610010015.png]]

#### Solution 1: (ChatGPT)

```
def create_door_mat(N, M):
    if N % 2 == 0 or M != 3 * N:
        print("Invalid size. N should be an odd number and M should be 3 times N.")
        return

    pattern = ".|."
    middle_text = "WELCOME"

    # Top part
    for i in range(1, N, 2):
        print((pattern * i).center(M, "-"))

    # Middle row
    print(middle_text.center(M, "-"))

    # Bottom part
    for i in range(N - 2, -1, -2):
        print((pattern * i).center(M, "-"))


# Example usage
N, M = input().split(" ")

N = int(N)
M =int(M)
create_door_mat(N, M
```