#### Source:
[GFG](https://www.geeksforgeeks.org/resource-allocation-graph-rag-in-operating-system/)
[JTP](https://www.javatpoint.com/os-resource-allocation-graph)
[YT](https://www.youtube.com/watch?v=AGZr5LaiyMg&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=45)




**Deadlock detection algorithm after assigning resources to the process, OS will check there is any deadlock or not
During **

#### About Resource allocation graph:

* It is used to detect a deadlock in OS.

![[Pasted image 20230517195836.png]]

* In resource allocation graph
	* P4 process wait for R2 resource but it assigned to P1
	* P3 process wait for R5 resource but it assigned to P4 process
		* Like these all process is waiting for another resources to perform a operation but some process take that resource, major issue here resources took process also wait for another resource, it lead to no progress between process, in this situation called deadlock
* We can simply use **wait for graph** to identify there is a dead lock or not in running process
	* In wait for graph we need to remove resources and looking process only
		* There we have a cycle look like shown in image then there is a deadlock
