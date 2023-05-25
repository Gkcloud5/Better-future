#### Source:
[YT](https://www.youtube.com/watch?v=rsp0rBP61As&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=74)

* We are using slab allocation method to allocate a memory for kernel objects.
* Some Kernel objects,
	* Process descriptors
	* Semaphore
	* File objects
* Slab is a collection of contiguous memory.
* caches is a collection of slab.
* Generally, slab contains pages.

![[Pasted image 20230525193927.png]]