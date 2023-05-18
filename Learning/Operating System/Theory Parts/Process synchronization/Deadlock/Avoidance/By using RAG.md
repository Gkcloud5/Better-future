#### Source:
[YT](https://www.youtube.com/watch?v=XV_U8feLJqQ&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=42)


#### Deadlock avoidance by using resource allocation graph:

* This method is used when process have single resource.
* Here we are using several type of edges
	* Claim edge
	* Request edge
	* Assignment edge == Allocated edge
* **Claim Edge:** it specifies that process may request a resource for future.
* **Request Edge:** whenever process wants to use resource, it request to resource.
* **Assignment Edge:** If resources is free then OS will allocate a corresponding resources to the process.
* Once process is completed then resources will be released.

![[Pasted image 20230518210136.png]]

