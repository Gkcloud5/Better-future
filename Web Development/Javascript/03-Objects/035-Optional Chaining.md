### 035-Optional Chaining ?.

* It is the safest way to access nested object properties.

```
let userAdmincheck = {
	admin() {
	console.log("i am chaining check admin")
	return 5
	}
	
  };
  
  let userGuest = {}
  userAdmincheck.admin?.();
  userGuest.admin?.();
  userGuest.admin;
  console.log(userGuest.admin?.(), userGuest.admin)
  console.log(userAdmincheck.admin?.())
```
![[Pasted image 20230731233706.png]]
