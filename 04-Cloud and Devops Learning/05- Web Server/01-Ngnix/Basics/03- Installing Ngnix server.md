
```
#installing in ubuntu 20
apt update
apt install nginx
systemctl start nginx
systemctl enable nginx
systemctl status nginx
```

### Basic configuration:

#### 1. Create a configuration file for website:
* Create new file in following directory
```
/etc/ngnix/site-available/mywebsite
```

#### 2. Configure the server block:
```
nano mywebsite

server {
	listen 80;
	server_name mywebsite.com www.mywebsite.com

    root /var/www/mywebsite; //root directory of website files

	index index.html; //Default index file

	location / {
		try_files $uri $uri/ =404;
	}
}
```

