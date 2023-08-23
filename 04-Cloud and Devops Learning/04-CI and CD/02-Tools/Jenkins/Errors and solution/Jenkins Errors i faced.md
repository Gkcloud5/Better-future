
#### 1.  Error 1: (ERROR: Build step failed with exception)

```
[DeployPublisher][INFO] Deploying /var/lib/jenkins/workspace/webAppExample/target/webappExample.war to container Tomcat 8.x Remote with context webAppExample

ERROR: Build step failed with exception
org.codehaus.cargo.container.ContainerException: Failed to redeploy
```

* Cargo library, which is used by Jenkins to manage container deployments, encountered an issue while trying to redeploy your application
* Reason for a error is 
	* context path, name should be case sensitive
	* and tomcat URL looks like `http://localhost:9090`
* 