#### Source:
[JTP](https://www.javatpoint.com/os-sjf-scheduling)
[GFG](https://www.geeksforgeeks.org/program-for-shortest-job-first-or-sjf-cpu-scheduling-set-1-non-preemptive/)
[YT](https://www.youtube.com/watch?v=MS5EPNUFx4o&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=23)

#### What is SJF in OS and why we need it?

* Shortest job first
* In this scheduling algorithm, it selects process as per the CPU burst time, which process has minimum burst time this scheduler will select for execution.
* It is reduce average waiting time of processes in the ready queue, also it minimizes the average turnaround time and maximizes the CPU utilization.
* Major drawback of SJF is starvation for long process, let consider if one process have a high burst time then chances for executing that process is very very hard here
* SJF is non-preemptive scheduling algorithm.