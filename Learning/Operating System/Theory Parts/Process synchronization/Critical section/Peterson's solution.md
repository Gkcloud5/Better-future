#### Source:
[YT](https://www.youtube.com/watch?v=uj-zhs7cUSI&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=32)
[GFG](https://www.geeksforgeeks.org/petersons-algorithm-for-mutual-exclusion-set-1/)

#### About Peterson's solution:

* It is a software solution of critical section.
* Software means program, it's a collection of instruction.
* We can use peterson's solution only 2 process are involved in critical section

![[Pasted image 20230515213544.png]]

##### Example:

```
bool flag[2];
int turn;

process Process0 {
    flag[0] = true;
    turn = 1;

    while (flag[1] && turn == 1) {
        // Wait until it's Process 0's turn
    }

    // Critical section
    // Access the shared resource

    flag[0] = false;
}

process Process1 {
    flag[1] = true;
    turn = 0;

    while (flag[0] && turn == 0) {
        // Wait until it's Process 1's turn
    }

    // Critical section
    // Access the shared resource

    flag[1] = false;
}

```


#### 3 requirements to solve critical section issue:

##### Mutual Exclusion:

* Critical section should have only one process at a time
* 