#### Source:
[GFG](https://www.javatpoint.com/os-disk-scheduling)

* Process needs two type of time
	* CPU time
	* IO time
		* It requests the OS to access the disk
* The OS must be fare enough to satisfy each request and at the same time, OS must maintain the efficiency and speed of process execution.
* The technique that OS uses to determine the request which is to be satisfied next is called disk scheduling.

#### Seek Time:

* Seek time is the time it takes a hard disk drive to move the read/write head to the correct location on the disk platter to access data.
* Seek time is one of the factors that determines the overall access time of a hard disk drive.


#### Rotational Latency:

* It is the time taken by the desired sector to rotate itself to the position from where it can access the R/W heads.
* **Platter** is a circular magnetic plat that is used for storing data in a hard disk.
* Rotational latency is the time it takes for a hard disk drive to rotate the platters until the desired data is under the read/write head. it is measured in ms.


#### Transfer time:

* It is the time taken to transfer a data

#### Disk Access time:

* Disk access time = Rotational latency + Seek time + transfer time

#### Disk response time:

* It is the average of time spent by each request waiting for the IO operations.


### Purpose Disk Scheduling:

* 