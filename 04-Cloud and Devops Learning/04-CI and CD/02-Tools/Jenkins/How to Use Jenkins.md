---
creation date: 2023-08-10 18:38
modification date: Thursday 10th August 2023 18:38:14
---

**Tags:** #DevOps 

#### Source:
[CG](https://chat.openai.com/share/ecb51290-7dea-4e7a-a57c-7a94f5506b6b)

--------------------------------------

### Explanation about it:

**Jenkins is a popular open-source automation sever that us used for buildings, testing and deploying software projects.**

* ##### 1. Installation and setup:
	* Access Jenkins after installed tool
		* http://IPaddress:8080
* ##### 2. Initial setup:
	* Use logs password to login and change password in setup page
	* Install recommended plugins
* ##### 3. Creating a new job:
	* Create a new job to build pipeline.
	* Choose type of job you want to create.
	* Most common types are
		* Freestyle project - Simple tasks
		* Pipeline - More complex workflows
* ##### 4. Configuring a freestyle project:
	* Give your project a name and choose project type
	* Configure source code management settings
		* Specifying the repo URL and auth credentials
	* Configure build triggers
		* Which can manual triggering
		* Scheduled builds
		* Or triggers from external systems
* ##### 5. Defining Build steps:
	* Add build steps to projects
		* It include
			* Compiling code
			* Running tests
			* Generating Documentation
			* etc
	* Configure post-build actions
		* Archiving artifacts
		* Sending notifications
		* Triggering other jobs
* ##### 6. Pipeline Setup:
	* If we are using a pipeline, we need to define build process in jenkins file
		* It's stored in version control system.
	* Jenkinsfiles are written in Groovy scripting language
	* Pipeline can have stages, steps and various syntax constructs for more complex workflows
* ##### 7. Running Jobs:
	* Manually trigger a job by clicking on a "Build Now"
	* Or setup automated triggers
* ##### 8. Viewing Build Results:
	* Once build is triggered, we can monitor its progress on dashboard
	* View build logs, console output
* ##### 9. Plugins and Extensibility:
	* Jenkins has a vast collection of plugins that enhance its capabilities.
	* You can install plugins to integrate with version control systems\
		* Testing frameworks
		* Deployment Tools
* ##### 10. Managing Jenkins:
	* Jenkins provides tools for managing users
		* Security settings
		* System Configuration

### [Uses](https://www.jenkins.io/doc/book/using/)


#### [[01-Jenkins - Practical knowledge]]
