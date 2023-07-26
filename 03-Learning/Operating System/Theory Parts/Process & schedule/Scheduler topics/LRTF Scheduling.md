#### Source:
[GFG](https://www.geeksforgeeks.org/longest-remaining-time-first-lrtf-cpu-scheduling-program/)

#### What is LRTF and why we need it?

* Longest remaining time first
* It is preemptive scheduling algorithm
* In the LRTF scheduling algorithm, the process with the longest remaining execution time is given the highest priority and is executed first.
* This approach minimize the average waiting time for processes and maximize CPU utilization by focusing on completing the longest-running process early.
* This scheduling algorithm also having a starvation issue.
* If two process have the same burst time then the FCFS will be used to get process from job queue.