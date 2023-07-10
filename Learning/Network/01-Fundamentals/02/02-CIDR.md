---
creation date: 2023-07-08 18:53
modification date: Saturday 8th July 2023 18:53:03
---

**Tags:** #network 

#### Source:
[AZ](https://aws.amazon.com/what-is/cidr/#:~:text=Classless%20Inter%2DDomain%20Routing%20(CIDR,IP%20address%2C%20associated%20with%20it.)

--------------------------------------

### What it is:

* **Classless Inter-Domain Routing.
* It is an IP address allocation method that improves data routing efficiency on the internet.
* Organizations use CIDR to allocate IP addresses flexibly and efficiently in their networks.
* Organization purchase three [[Class in IP address|classes]] of IPv4 address
* CIDR is a classless addresses
	* It use [[VLSM]](Variable length subnet masking) to alter the ration between the network and host address bits in an IP address.
* A CIDR IP address appends a suffix value starting the number of network address prefix bits to a normal IP address.
	* EXAMPLE: 192.0.2.0/24 is an IPv4 CIDR address.


### Benefits of CIDR:
##### Reduce IP address wastage:
* CIDR provides flexibility when you determine the network and host identifier assignments on an IP address.
* You can use CIDR to provision the required number of IP addresses for a particular network and reduce wastage.
* CIDR reduces routing table entries and simplifies data packet routing.

##### Transmit data quickly:
* CIDR allows routers to organize IP addresses into multiple subnets more efficiently.
* A subnet is a smaller network that exist within in a network.
	* All device connected to a router are on the same subnet and have the same IP address prefix.

##### Create a Virtual private cloud:
* A VPC is a private digital space hosted within the cloud.
* It allows your organization to provision workload