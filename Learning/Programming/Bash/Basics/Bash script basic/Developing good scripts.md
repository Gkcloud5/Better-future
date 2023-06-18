---
creation date: 2023-06-18 17:41
modification date: Sunday 18th June 2023 17:41:59
---

**Tags:** #linux #bash

#### Source:
[bash](https://tldp.org/LDP/Bash-Beginners-Guide/html/sect_01_05.html)

--------------------------------------

#### Explanation about it:

##### Properties of good scripts:

* A script should run without errors.
* It should perform the task for which it is intended
* Program logic is clearly defined  and apparent
* Script does not do unnecessary work
* Script should be reusable.

##### Structure:

* Structure of a shell script is very flexible.
* we must ensure correct logic, flow control and efficiency so that users executing the script can do so easily and correctly
* When a starting on a new script, ask yourself the following question
	* Will I be needing any information from the user or from the user's environment?
	* How will I store the information?
	* Are there any files that need to be created? where and with which permissions and ownerships?
	* What commands will I use? when using the script on different systems, do all these systems have these commands in the required versions?
	* Does the user need any notifications? when and why?

##### Terminology:

![[Pasted image 20230618175718.png]]

**Using our own spoken language to pin down the tasks to be executed by our program will help us to create an understandable form of our program**

###### Example logic flow:

```
1. Do you want to rotate logs?
    
    1. If yes:
        
        1. Enter directory name containing the logs to be rotated.
            
        2. Enter base name of the log file.
            
        3. Enter number of days logs should be kept.
            
        4. Make settings permanent in user's crontab file.
            
    2. If no, go to step 3.
        
2. Do you want to rotate another set of logs?
    
    1. If yes: repeat step 1.
        
    2. If no: go to step 3.
        
3. Exit
```
