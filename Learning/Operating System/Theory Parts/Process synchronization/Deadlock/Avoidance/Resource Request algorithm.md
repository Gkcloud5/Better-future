#### Source:
[YT](https://www.youtube.com/watch?v=GUnNgMgQlGo)
[YT-2](https://www.youtube.com/watch?v=bIX2MTwsUDc)


#### About algorithm:

* this algorithms will help whether request resource is allocated or not.
* If a process request for some resource
	* If `request <= max need` then goes to next step
	* If `request <= avilable resource`, once satisfied then went to next step
	* Allocate the requested resources to process by modifying
		* Available = Available - request
		* Allocation = Allocation + request
		* Need = Need - request
	* If safe state ==> then resource allocated
	* If unsafe state ==> Then resources not allocated