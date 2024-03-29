
### Source:
1. [CG](https://chat.openai.com/share/5d0d0db7-f63f-4eaf-a0c5-428cb417ad30)

### 1. Basic system information:
* `uname -a` : Display kernel and system information
* `hostnamectl`: Provides detailed information about the system hostname and OS
* `lsb_release -a`: Shows distribution-specific information

### 2. CPU information:
* `lscpu` : Provides detailed information about the CPU architecture, cores and capabilities
* `cat /proc/cpuinfo` : Displays detailed information about each CPU core

### 3. Memory information:
* `free -h`: shows memory usage and information in human readable format
* `cat /proc/meminfo` : Display detailed memory information

### 4. Disk and Filesystem information:
* `df -h` : Display disk space usage of mounted filesystem
* `du -h <directory>` : shows disk usage of specific directory
* `lsblk` : List block devices and related information

### 5. Network information:
* `ifconfig` : display network information
* `netstat -tuln` : Shows active network connections

### 6. System load and processes:
* `top` : provides a dynamic view of system processes, resource usage and system load
* `ps aux` : list detailed information about running processes
* `htop` : A more user friendly alternative to `top`

### 7. Kernel and Modules:
* `lsmod` : List loaded kernel modules
* `modinfo <module name>` : Display information about a specific kernel module

### 8. User and group information:
* `id <username>` : Shows information about a specific user
* `groups <username>` : Lists groups a user belongs to
* `cat /etc/passwd` : Display user account information

### 8. System Logs:
* `dmesg`: Displays kernel ring buffer messages
* Log files in `/var/log` : Various logs for different services can be found here

