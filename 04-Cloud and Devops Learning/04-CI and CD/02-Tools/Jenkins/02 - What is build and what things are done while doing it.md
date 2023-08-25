
### Source:
[CG](https://chat.openai.com/share/7d5f9b08-ba5a-4aa3-b8b8-c67fbc18f86f)

**Build refers to the process of compiling, testing and packaging source code into a deployable artifact.**

#### Steps involved in build process:

##### 1. Source Code Retrieval: 
* Jenkins pulls the source code from version control

##### 2. Compile and Build:
* Converting source code into executable binaries or other intermediate forms

##### 3. Testing:
* Automating test process.
	* Unit tests
	* Integration tests

##### 4. Static Analysis:
* Used to identify code quality issues, potential vulnerabilities.
* Adherence to coding standards

##### 5. Packaging:
* After successful compilation and testing, Jenkins may package the code and its dependencies into deployable artifact.
	* JAVA files will be JAR or WAR file

##### 6. Deployment:
* Deployment in test or production environment.

##### 7. Reporting:
* Jenkins collect various data such as test results, code metrics and static analysis reports.

##### 8. Notifications:
* Jenkins can send notification to developers

##### 9. Trigger Builds:
* Je