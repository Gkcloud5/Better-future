---
creation date: 2023-07-18 17:10
modification date: Tuesday 18th July 2023 17:10:48
---

**Tags:** #network 

#### Source:
[GFG](https://www.geeksforgeeks.org/tcp-3-way-handshake-process/)

--------------------------------------

#### Explanation about it:

![[Pasted image 20230718171146.png]]

* In TCP connection made after 3-way handshake is made.


#### Step 1: (SYN)
* First client sends a segment with SYN(Synchronize sequence number)which informs the server that the clients is likely to start communication and with what sequence number it starts segments with.

#### Step 2 (SYN+ACK):
* Server responds to the client request with SYN-ACK signal bits set.
* ACK(Acknowledgement) signifies the response of the segment it received and SYN signifies with what sequence it is likely to start the segments with.

#### Step 3 (ACK):
* In the final part client acknowledges the response of the server and they both establish a reliable connection with which they will start the actual data transfer.