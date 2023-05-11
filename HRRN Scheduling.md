#### Source:
[GFG](https://www.geeksforgeeks.org/highest-response-ratio-next-hrrn-cpu-scheduling/)

#### What is HRRN Scheduling?

* Highest response ratio next
* It is a non-preemptive algorithm.
* In HRRN, OS need to find the response ratio of all available processes and select the one with the highest response ratio. a process once selected will run till completion.
* Here scheduling is done on the basis of an extra parameter called response ratio.
* A response ratio is calculated for each of the available jobs and the job with the highest response ratio is given priority over the others.

```
 Response Ratio = (W+S)/S
```

W --> Waiting time
S  --> Service time or burst time

