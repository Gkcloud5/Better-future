#### Source:
[GFG](https://www.geeksforgeeks.org/operating-system-sleeping-barber-problem/)

#### Explanation about problem:

* There is Barbour shop with one barber and n number of chairs for waiting customers
	* Customer arrives at random times and if there is an available chair, they take a seat and wait for the  barber to become available.
	* If there no chairs available, the customer leaves.
	* when the barber finishes with customer
		* He checks if there are any waiting customers.
			* If there are, he begins cutting the hair of the next customer in the queue.
			* If there are no customers waiting, he goes to sleep.
