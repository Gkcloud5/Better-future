#### Source:
[YT](https://www.youtube.com/watch?v=mWO0XazqV9g&list=PLXj4XH7LcRfDrdQuJTHIPmKMpa7eYVaPm&index=30)

#### What is producer and consumer problem:
* Here we have two process
	* Producer
	* Consumer
* Producer process produced a item and consumer process will consume it.
* Shared buffer is shared between producer and consumer

![[Pasted image 20230512215011.png]]

Count --> Shared variable.

* Size of a buffer is 5.
* Producer produce a item and put it in buffer.
	* Before storing a buffer we need to check buffer is full or not.

#### Problem:

![[Pasted image 20230513163545.png]]

