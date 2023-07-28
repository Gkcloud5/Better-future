---
creation date: 2023-07-27 16:36
modification date: Friday 28th July 2023 13:37:49
---

**Tags:** #network 

#### Source:
[Latency](https://www.cloudflare.com/learning/performance/glossary/what-is-latency/)

--------------------------------------

### What it is:

* Latency is the time takes for data to pass from one point on a network to another.
* Most often, latency is measured between a user's device to data center
* This measurement helps developers understand how quickly a webpage or application will load for users.
* Data transfer internet on speed of light.

### What causes internet latency?

* One of the things is **distance**
* [[Round trip in network]]
	* RTT is equal to double amount of latency

### Network latency, throughput and bandwidth:

* All are interrelated, but they all measure different things
* **Bandwidth** is the maximum amount of data that can pass through the network at any given time.
* **Throughput** is the average amount of data that actually passes through over a given period of time.
* **Latency** is a measurement of time, not of how much data is downloaded over time.

#### How can latency be reduced?

* CDN is a major steps to reduce a latency.
* Minimize the number of render-blocking resources
	* JS related changes
	* Optimize images
	* Reduce code size


