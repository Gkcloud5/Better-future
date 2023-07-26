#### Source:
[GFG](https://www.geeksforgeeks.org/multilevel-feedback-queue-scheduling-mlfq-cpu-scheduling/)
[YT](https://www.youtube.com/watch?v=EsXBdY35ieA&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=29)

#### What is multilevel feedback queue?

* It almost same like MLQ, it is designed to handle processes with varying characteristics and dynamic priority adjustments based on their behavior.
* In this algorithm, ready queue divided into multiple queues, each with a different priority level. the queues are ordered in terms of priority.
* Key feature of multi level feedback queue is that it allows processes to move between queue based on their behavior. 
* The priority of the process can be adjusted dynamically based on its behavior, such as how much CPU time it has used or how often it has been blocked. 

![[Pasted image 20230511230717.png]]

