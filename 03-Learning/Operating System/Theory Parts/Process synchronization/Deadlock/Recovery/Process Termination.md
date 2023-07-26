#### Source:
[YT](https://www.youtube.com/watch?v=kOYTmxKpIms&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=47)


**Once deadlock is detected we can use process termination method to recover a process from deadlock**

#### 2 Technique:

##### 1.  Abort all deadlock process:

* Out of 10 process 3 process are suffering with deadlock, so we need to eliminate the 3 process which are suffering from deadlock
* Disadvantage of this process is
	* In 3 process if they are completed almost 80 to 90% after that they suffering from deadlock, inorder to use this method they will kill 3 process so till now this process takes so much CPU time and some other resources time to complete 80%, all will be waste.

##### 2. Abort 1 process at a time until deadlock is eliminated:

* out of 10 process only 3 process suffering from deadlock, inorder to use this method.
* First it will remove one of the deadlock suffering process and use deadlock detection algorithm to know still deadlock is present or not
* Still it present then will kill another deadlock suffered process and then use deadlock detection process to find still deadlock is there are not
* It continues until deadlock gone.
* Disadvantage of the process is:
	* If 100 process is suffered from deadlock by using this method will take so much time to recover a deadlock, incase last process is a main cause for deadlock