#### Source:
[TP](https://www.tutorialspoint.com/unix/unix-file-permission.htm)


* File permission is important of linux that provides a secure method for storing files.
* **Owner permission:**
	* The owner's permission determine what actions the owner of the file can perform on the file
* **Group Permissions:** 
	* Group permission's determine what actions a user. who is a member of the group that a file belongs to, can perform on the file.
* **other permissions:**
	* The permissions for others indicate what action all other users can perform on the file


#### Permission indicators:

```
ls -l /home/

#output 
-rwxr-xr--  1 amrood   users 1024  Nov 2 00:10  myfile
drwxr-xr--- 1 amrood   users 1024  Nov 2 00:10  mydir
```

* First column represents different access methods, permission associated with a file or a directory.
* The important things
	* **read(r)**
	* **write(w)**
	* **execute(x)**
* 2 to 4 character represents permission for the file's owner.
	* -rwxr --> owner had read, write and execute permission
* 5 to 7 consists of the permission for the group to which the be