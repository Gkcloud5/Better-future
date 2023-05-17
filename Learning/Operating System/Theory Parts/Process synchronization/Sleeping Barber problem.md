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


#### Theoretical example:

-   Each barber has a semaphore that is initially set to 0.
-   When a customer arrives at the barbershop, he decrements the semaphore of the first barber in line.
-   If the semaphore is greater than 0, the customer enters the barber's room and gets a haircut.
-   If the semaphore is 0, the customer waits in the waiting room.
-   When the barber finishes serving a customer, he increments the semaphore.
-   If there are any customers waiting in the waiting room, the barber wakes up and serves the next customer.


#### Example programme:

##### Barber process:

``` python
while True:
    # Check if there are no customers
    if customer_semaphore.value == 0:
        # Barber falls asleep
        sleep()

    # Acquire customer semaphore
    wait(customer_semaphore)

    # Acquire mutex to update shared variables
    wait(mutex)

    # Increment available chairs
    n += 1

    # Release mutex
    signal(mutex)

    # Signal barber semaphore to indicate readiness
    signal(barber_semaphore)

    # Cut hair
    cut_hair()

```

##### Customer process:

``` python
# Acquire mutex to update shared variables
wait(mutex)

# Check if there is an available chair
if n > 0:
    # Decrement available chairs
    n -= 1

    # Signal customer semaphore to indicate arrival
    signal(customer_semaphore)

    # Release mutex
    signal(mutex)

    # Acquire barber semaphore
    wait(barber_semaphore)

    # Get a haircut
    get_haircut()
else:
    # Release mutex
    signal(mutex)

    # Leave the barber shop
    leave()

```