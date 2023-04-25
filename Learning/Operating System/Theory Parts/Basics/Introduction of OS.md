#### Source:
[Intro](https://www.geeksforgeeks.org/introduction-of-operating-system-set-1/)

#### About OS:

* An OS acts as an intermediary between the user of a computer and computer hardware.
* Purpose of OS is an to provide an environment in which a user can execute programs conveniently and efficiently.
* An OS is software that manages computer hardware.

#### Definition of OS:

* An OS is a program that controls the execution of application programs and acts as an interface between the user of a computer and the computer hardware.
* A more common definition is that the OS is the one program running at all times on the computer(Usually called the kernel). 
* An OS is concerned with the allocation of resources  and services, such as
	* Memory
	* Processors
	* Devices
	* Information


#### Features of OS:

* An OS makes a computer more **convenient** to use.
* An OS allows the computer system resources to be used **efficiently**
* OS give maximum **Throughput** (No.of tasks per unit time)


#### Functions of OS:

* **Resources Management:
	* OS need to allocate a resources as per the process and need to decide how long it want to there in CPU 
* **Process Management:**
	* OS do scheduling a process and terminate a process.
* **Storage Management**
	* File system mechanism used for the management of the storage.
* **Memory Management**
	* OS need to decide how much memory has been used and by whom. it has to decide which process needs memory space and how much.
	* OS has to allocate and deallocate the memory space.
* **Security/Privacy Management**
	* Privacy also provided by the OS


#### Working skeleton of OS:

User --> System and application program --> OS --> Hardware

* Hardware consists of memory, CPU, ALU, I/O devices, peripheral devices and storage devices.

![[Pasted image 20230425003820.png]]



#### OS Designed for:

* It controls the allocation and use of the computing system's resources among the various user and tasks
* It provides an interface between the computer hardware and the programmer that simplifies and makes it feasible for coding

#### I/O system Management:

 * The module that keeps track of the status of devices is called the I/O traffic controller.
	* Each I/O device has a device handler that resides in a separate process associated with that device.
	* [Youtube](https://www.youtube.com/watch?v=tVjoQ7sdrY8)
	* OS manages communication with the devices through their respective drivers


![[Pasted image 20230425005054.png]]


#### Types of OS:

* **Batch OS:**
	* A collection of jobs. user uses punch cards for executing program.
	* CPU idle time is high here
* **Time Sharing OS:**
	* It allows many users to share computer resources.
* **Distributed OS:**
	* It manages a group of different computers and makes appear to be a single computer.
* **Network OS:**
	* Computer running in different OS can participate in a common network.
* **Real-time OS:**
	* It is used to execute real time application.


#### Feature of OS:

* **Memory Management:**
	* OS manages the computer's memory, ensuring that program have the necessary memory to run and allocating memory efficiently to maximize performance.
* **Process Management:**
	* OS is a responsible for managing the processes running on the computer. it schedules process to run on the CPU, allocates system resources to processes and terminates processes when they are no longer needed.
* **File System Management:**
	* OS is responsible for storing and retrieving a data from hard disk or any other storage devices.
* **Device Management:**
	* OS manages the computer input and output devices such as keyboard and mouse. ensuring that they are properly configured and functioning correctly.
* **Security:**
	* OS provides security feature to protect the computer from unauthorized access, viruses
* **User interface:**
	* OS provides GUI or command line interface to interact with the computer. 
