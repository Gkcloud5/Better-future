
#### 1.  Error 1: (ERROR: Build step failed with exception)

```
[DeployPublisher][INFO] Deploying /var/lib/jenkins/workspace/webAppExample/target/webappExample.war to container Tomcat 8.x Remote with context webAppExample

ERROR: Build step failed with exception
org.codehaus.cargo.container.ContainerException: Failed to redeploy
```

* Cargo library, which is used by Jenkins to manage container deployments, encountered an issue while trying to redeploy your application

```
#Clear cargo plugin commands
<build>
    <plugins>
        <plugin>
            <groupId>org.codehaus.cargo</groupId>
            <artifactId>cargo-maven2-plugin</artifactId>
            <version>1.8.4</version> <!-- Use the appropriate version -->
            <configuration>
                <!-- Configure the container type, URL, and deployment settings -->
                <container>
                    <containerId>tomcat9x</containerId> <!-- Use the appropriate container ID -->
                    <type>remote</type>
                </container>
                <configuration>
                    <type>runtime</type>
                    <properties>
                        <!-- Container-specific properties -->
                        <cargo.hostname>localhost</cargo.hostname>
                        <cargo.remote.username>admin</cargo.remote.username>
                        <cargo.remote.password>admin</cargo.remote.password>
                    </properties>
                </configuration>
                <deployer>
                    <type>remote</type>
                </deployer>
                <deployables>
                    <deployable>
                        <groupId>com.example</groupId>
                        <artifactId>your-app</artifactId>
                        <type>war</type>
                        <properties>
                            <context>your-context-path</context>
                        </properties>
                    </deployable>
                </deployables>
            </configuration>
        </plugin>
    </plugins>
</build>
```

