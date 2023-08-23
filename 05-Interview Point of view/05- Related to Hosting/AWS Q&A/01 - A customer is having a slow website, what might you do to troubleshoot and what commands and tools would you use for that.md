
### Sources:
1. [LW](https://www.liquidweb.com/kb/how-to-troubleshoot-a-slow-loading-website/)
2. [CG](https://chat.openai.com/share/1a42cc47-cfd9-46cd-930d-6f8d851e7c32)
### Reason for slowness:

* First we need to measure the website performance, for that following websites will useful for it
	* [Pagespeed Insights](https://developers.google.com/speed/pagespeed/insights/)
	* [Websitetest](https://webpagetest.org/)
	* [GTMetrics](https://gtmetrix.com/)
* Some other things for client feel slowness
	* Distance
	* Network speed
	* Routing issues
	* Computer speed
* Performance Metrics:
	* First Contentful paint
	* Speed Index
	* Largest Contentful paint
	* Time to interacive
* Browser Timings:
	* Redirect Duration
	* Connection Duration
	* Backend Duration
	* First Paint
	* DOM
	* Onload time
* Area of issues:
	* Website code
	* CMS related optimizations
	* Website concerns
		* Scripts
		* Disable hotlinking
	* OS/Server Problems
	* Hosting issues

#### OS/Server Problems:

##### 1. Server Health Check:
* use `top` command to monitor
	* CPU
	* Memory
	* Process usage

##### 2. Keep server update:
* Keep server software updated
	* Apache
	* CMS
	* PHP

##### 3. Network connectivity:
* use `ping` command
	* Time is high or there's packet loss then it might indicate network connectivity issues
* Use `traceroute` command
	* It shows path that data takes from local to website server, it include time taken at each hop
	* You can get where it take so much time
* 