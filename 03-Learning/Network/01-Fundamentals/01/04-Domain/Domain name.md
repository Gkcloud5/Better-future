---
creation date: 2023-07-05 18:30
modification date: Wednesday 5th July 2023 18:30:55
---

**Tags:** #network 

#### Source:
[DN](https://www.cloudflare.com/learning/dns/glossary/what-is-a-domain-name/)

--------------------------------------

### What it is:

* A domain name is a string of text that maps to an alphanumeric IP address.
* It used to access a website from client software

`A domain name is the text that a user types into a browser window to reach a particular website.`

* The actual address of a website is a complex numerical IP address so that only we use domain name to reach website easily.
* By using [[DNS in Networking|DNS]] system get IP address of domain name.


### Who manages domain names?

* Domain names are all managed by [[Domain Registries]].
* Anyone who wants to create a website can register a domain name with a registrar, and there are currently over 300million registered domain names.

### What is the difference between a domain name and URL?

* URL --> **Uniform resource locator**, sometime called a web address.
	* It contain domain name of  site as well as other information, including
		* Protocol
		* Path
* Example:
	* `https://cloudfare.com/learning/` 
		* `cloudfare.com` is a domain name
		* [[https]] is a protocol
		* `learning` is a specific path

### What are the parts of a domain name?

* Domain name typically broken up into two or three parts, each separated by a dot. when right to left 
	* [[Top level domain]]
		* .com
		* .net
		* .org
	* 2nd thing from left of the TLD
		* .co
		* google
		* Example:
			* google.co.uk
			* here `.co` is a 2LD(2nd level domain)
	* On left from 2LD is called 3LD
		* from above example `google` is a 3LD

