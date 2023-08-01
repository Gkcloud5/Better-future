---
creation date: 2023-08-01 18:11
modification date: Tuesday 1st August 2023 18:11:22
---

**Tags:** #DevOps 

#### Source:
[CG](https://chat.openai.com/share/3f3d639a-8fa9-43c8-9449-e584035233cf)

--------------------------------------

## Explanation about it:

### 1. About continuous integration:

 * CI is the practice of frequently integrating code changes from multiple developers into a shared repository.
 * Main goal is to catch integration issues early by automating the process of building and testing the application whenever new code is pushed to the repo.

##### 1.1 Automation:
 * Setup automated build and test processes to be triggered automatically on code commits.

##### 1.2 Frequent Integration:
 * Developers should frequently merge their code changes into the main branch to avoid large, complex merges and identify conflicts early.

##### 1.3 Fast Feedback:
 * CI helps provide rapid feedback to developers, identifying issues in code and test cases quickly.

##### 1.4 Version Control:
 * Version Control systems, like GIT, are crucial for effective CI, as they enable collaboration and tracking of changes.

### 2. Most using CI tools:
**Tools used to automate the building, testing and reporting processes**
 * Jenkins
 * Gitlab CI/CD
 * Travis CI

### 3. [[Learning Version Control]]


### 4. Continues Deployment:
 * CD extends CI by automating the deployment process of applications to production or staging environments.
 * Goal is ensure that the application is always in a deployable state, enabling faster and more reliable releases.

##### 4.1 Continuous Deployment:
 * Here code change automatically deployed to production without manual intervention.

##### 4.2 Continuous Delivery:
 * In this approach, code change automatically deployed to a staging environment. then it awaits manual approval for deployment to production.

##### 4.3 Key concepts and practices for CD:
 * **Infrastructure as Code(IaC):
	 * Use tools like terraform or AWS cloudformation
		 * To define and manage infra in version controlled and automated manner.
* **Deployment pipelines:**
	* Design automated pipelines that include
		* Building
		* Testing
		* Deploying application through various stages