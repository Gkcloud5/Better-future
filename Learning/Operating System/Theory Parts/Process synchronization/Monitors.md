#### Source:
[YT](https://www.youtube.com/watch?v=YUzuMxy2NQ0&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=91)
[GFG](https://www.geeksforgeeks.org/monitors-in-process-synchronization/)

#### About monitors:

* Monitors is alternative to semaphore.
* it vey helpful inorder to provide process synchronization.
* Monitors are implemented as programming language constructs.

![[Pasted image 20230515191120.png]]

* a monitor is a synchronization construct that combines 
	* Shared data
	* Procedures
	* Condition variable
* Monitors provide high level abstraction for concurrent programming. making it easier to manage shared resources and ensure mutual exclusion.
* Example

```
Monitor BankAccount {
    int balance;

    procedure deposit(int amount) {
        balance += amount;
    }

    procedure withdraw(int amount) {
        if (amount <= balance) {
            balance -= amount;
        } else {
            // Wait until enough funds are available
            wait(withdrawCondition);
            balance -= amount;
        }
    }

    condition withdrawCondition() {
        return balance >= amount;
    }
}

```

* In above example **shared variable is balance** and **procedures are deposit and withdraw**, the **withdraw condition is a condition variable**

![[Pasted image 20230515194919.png]]

