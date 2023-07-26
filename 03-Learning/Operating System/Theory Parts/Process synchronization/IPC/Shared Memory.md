#### Shared Memory:

 ![[Pasted image 20230513225623.png]]

* We have 2 process p1 and p2 and have shared memory.
* It is very very faster because it don't need any system call.
* Here p1 can communicate with p2 with a help of shared memory.

##### Example for shared memory:
* Let assume producer and consumer problem,

![[Pasted image 20230514141954.png]]

in --> next free position
out --> first full position


![[Pasted image 20230514142219.png]]

* Communication between  processes using shared memory requires processes to share some variable, and it completely depends on how the programmer will implement it.
