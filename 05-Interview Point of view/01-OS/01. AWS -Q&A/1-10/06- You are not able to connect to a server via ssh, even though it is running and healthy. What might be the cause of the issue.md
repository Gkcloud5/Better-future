
### Some reasons:

##### 1. Related to Firewall:
* Need to check if firewall blocking any incoming SSH connections
* Ensure allocated port is open for incoming traffic
* Need to check if two firewall is active in server, if yes, need to stop one firewall

##### 2. SSH Configuration:
* Verify SSH server configuration
	* `/etc/ssh/sshd_config`
* Ensure that SSH is configured to listen on the correct network interface and port
* Need to check any restrictions or configuration that might prevent our connection
	* Permitrootlogin
	* Password authentication

##### 3. SSH Service Status:
* Confirm SSH service is running on the server
	* `systemctl status ssh`

##### 4. SSH Key issues:
* If we use public auth key, ensure that SSH key pair is correctly configured on both client and server sides
* Verify public key is added `~/.ssh/authorized_keys`

##### 5. Service Restart:
* Restart SSH service and check able to connect or not
	* `service ssh restart`

