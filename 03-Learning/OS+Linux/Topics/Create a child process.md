
**Process**

#### Source:
[YT](https://www.youtube.com/watch?v=7VOW4zkDZrQ&list=PL3uLubnzL2Tlbyrr2GFVRE7Azo8FJe-dJ&index=6)
[child](https://www.includehelp.com/operating-systems/child-process-in-operating-system.aspx)


#### What is a child process in OS?

* One process can create another process, this methodology involves in multitasking OS
	* Here, the process creates another process is called the parent process and created process is referred to as the child process.
* Child process is a subprocess of a main process

#### Approaches for creating a child process:

* Two Approaches
	* By using **fork** system call
	* By using **spawn** system call

##### Fork system call:

* Most of the features of the parent process come into its child process.
* For example,
	* File descriptors come into subprocess from its parent
* In the unix system, a child process is referred to as the copy of its parent, using the fork system call.
* After the child process has created, it can be laminated with a different program(using exec system call) as per the requirement.

##### By using the spawn:

* Spawn is a method by which we can load and execute a new child process. currently, the running process can wait for the subprocess bring to an end or it can continue on its job.
* Any process that is new to the system it requires sufficient memory space that's why parent and its subprocess can execute without any interruption.

#### Limitation to create child process:

* Each process can create many sub processes but each and every process must have parent process
	* If process does not have a parent process so this indicates it was directly created by the kernel
* Some process which has no parent may be created to carry out various daemon tasks in user space. 
	* A way by which process end up is death of it's parent. It leaves its child as a orphan process and with the sum up this process is adopted by **init** process.

#### End of a child process:

* When child process ends up its execution or terminates, some data is go back to its parent process.
* **Zombie:**
	* A zombie process is a process that has completed execution but still has an entry in the process table. this occurs for a child process.
	* as the parent process still needs to read its child exit status. once this is done using the **wait()** system call, then the zombie process is eliminated from the process table.

![[Pasted image 20230529183025.png]]



#### Program:

```C
#include <stdio.h>
#include <unistd.h>

int main() {
    pid_t pid = fork(); // Fork the current process

    if (pid < 0) {
        // Error occurred while forking
        fprintf(stderr, "Fork failed.\n");
        return 1;
    } else if (pid == 0) {
        // Child process
        printf("Hello from the child process!\n");
    } else {
        // Parent process
        printf("Hello from the parent process! Child's PID: %d\n", pid);
    }

    return 0;
}

```